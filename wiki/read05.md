# Heroku:
 #### Heroku is a PaaS (Platform as a Service) that enables language-agnostic hosting of web applications.
### **Jargon:**
* Application: Source Code, Dependency Description, [Framework
 
  - For Node.js the dependency description will take the form of a package.json.
  - The source code and dependency decription together should be enough for heroku to build an application. 
  
* Process Type: Executable program that handles specific work within the application. Process types are also the prototype from which dynos are instantiated. 

* Dyno: Instances of a specific Process Type. As the demand increases for a process type and concurrent instances must exist to handle the load the number of dynos will scale. 
  - The free version of heroku includes a single web and worker dyno. 
  - It also includes up to 1000 free hours of server runtime per month. 
  - ```herokus ps``` will provide a description of running dynos.
  - Each dyno also includes an ephemeral filesystem.
    + An epemeral filesystem can also be described as a scratchpad or internal data register. It is ephemeral in that it is only accessible to its contexual dyno.

* Slug: A prepacked and compressed object which contains everything needed for a single instance of the application. 

* Add-ons: I am less clear on how to describe these but they seem to be APIs accessible by heroku that import various other services. I notice that mongoDB and Postgres both have add-ons for Heroku.

* Dyno Manager: Built-in functionality for heroku to manage dynos on your behalf.

* Procfile: [Documentation](https://devcenter.heroku.com/articles/procfile) 
  - Heroku doesn't need procfiles for common frameworks but it is still a good idea to install them as a failsafe and for increased configuration control.
  - Procfiles must be included at the root directory.
  - Procfiles do not end in an extension.
  - Procfiles must follow the naming convention ```Procfile```
  - They are a text document composed of pairs like:
    + ```<process type>: <command>```

* Release: Each time you make a change to your deployed code or configuration files Heroku will log a new release. 

## References

[Node.js Application Deployment](https://devcenter.heroku.com/articles/getting-started-with-nodejs)


[My first Heroku app](https://evil-alien-88095.herokuapp.com/)
