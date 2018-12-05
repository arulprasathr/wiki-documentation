# Servlet lifecycle

- First the HTTP requests coming to the server are delegated to the servlet container.

- The servlet container loads the servlet before invoking the service() method.

- Then the servlet container handles multiple requests by spawning multiple threads, each thread executing the service() method of a single instance of the servlet.

![Servlet Lifecycle](http://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/arulprasathr/wiki-documentation/master/uml/servlet-lifecycle.txt)
