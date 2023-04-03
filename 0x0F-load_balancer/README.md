##  Load Balancer

HAProxy, which stands for High Availability Proxy, is a popular open source software TCP/HTTP Load Balancer and proxying solution which can be run on Linux, macOS, and FreeBSD. Its most common use is to improve the performance and reliability of a server environment by distributing the workload across multiple servers (e.g. web, application, database). It is used in many high-profile environments, including: GitHub, Imgur, Instagram, and Twitter.
A backend is a set of servers that receives forwarded requests. Backends are defined in the backend section of the HAProxy configuration. In its most basic form, a backend can be defined by:
- which load balance algorithm to use.
- a list of servers and ports.

A backend can contain one or many servers in it. Generally speaking, adding more servers to your backend will increase your potential load capacity by spreading the load over multiple servers. Increased reliability is also achieved through this manner, in case some of your backend servers become unavailable.

### HTTP Request Header

Whenever you type a URL into the address bar and try to access it, your browser sends an HTTP request to the server. The HTTP request header contains information in a text-record form, which includes particulars such as the:

- Type, capabilities and version of the browser that generates the request.
- Operating system used by the client.
- Page that was requested.
- Various types of outputs accepted by the browser.

### HTTP Response Header
Upon receiving the request header, the Web server will send an HTTP response header back to the client. An HTTP response header includes information in a text-record form that a Web server transmits back to the client's browser. The response header contains particulars such as the type, date and size of the file sent back by the server, as well as information regarding the server.

### HTTP General Header
These headers contain directives that need to be followed, for both the requester and receiver. This can include information regarding:
- Caching directives.
- Specified connection options.
- The date (always listed in Greenwich Mean TIme)
- Pragma
- Upgrade (for if the protocols need to be switched)
- Via (to indicate intermediate protocols)
- Warning (for additional information not found elsewhere in the header. There may be more than one warning listed.)

### HTTP Entity Header
These headers include information regarding:
- Allow (methods supported by the identified resource)
- Content Encoding.
- Content Language.
- Content Location.
- Content Length.
- MD-5 (for checking the integrity of the message upon receipt).
- Content Range.
- Content Type.
- When it Expires.
- When it was last modified.
