# Servlet lifecycle
A servlet life cycle can be defined as the entire process from its creation till the destruction. The following are the paths followed by a servlet.

- The servlet is initialized by calling the init() method.
- The servlet calls service() method to process a client's request.
- The servlet is terminated by calling the destroy() method.
- Finally, servlet is garbage collected by the garbage collector of the JVM.

![Servlet Lifecycle](http://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/arulprasathr/wiki-documentation/master/uml/servletlifecycle.txt)
