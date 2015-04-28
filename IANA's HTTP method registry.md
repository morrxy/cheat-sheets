# IANA's HTTP method registry <sup>[[source]](http://www.iana.org/assignments/http-methods/http-methods.xhtml)</sup>

**Safe** methods don’t modify resources.
**Idempotent** methods can be called many times without different outcomes.

Method name                             | Safe | Idempotent | Description
-----------                             | ---- | ---------- | -----------
[ACL][acl]                              | no   | yes        | Modifies the access control list (which can be read via the DAV:acl property) of a resource.
[BASELINE-CONTROL][baseline-control]    | no   | yes        | Places a collection under baseline control
[BIND][bind]                            | no   | yes        | Modifies the collection identified by the Request-URI, by adding a new binding from the segment specified in the BIND body to the resource identified in the BIND body.
CHECKIN [¹][checkin-1] [²][checkin-2]   | no   | yes        | 
[CONNECT][connect]                      | no   | no         | Requests that the recipient establish a tunnel to the destination origin server identified by the request-target and, if successful, thereafter restrict its behavior to blind forwarding of packets, in both directions, until the tunnel is closed.
[COPY][copy]                            | no   | yes        | Creates a duplicate of the source resource identified by the Request-URI, in the destination resource identified by the URI in the Destination header.
[DELETE][delete]                        | no   | yes        | Requests that the origin server remove the association between the target resource and its current functionality.
[GET][get]                             | yes  | yes        | Requests transfer of a current selected representation for the target resource.
[HEAD][head]                            | yes  | yes        | Identical to GET except that the server MUST NOT send a message body in the response (i.e., the response terminates at the end of the header section).
[LABEL][label]                          | no   | yes        | Can be applied to a version to modify the labels that    select that version.
[LINK][link]                            | no   | yes        | Establishes one or more Link relationships between the existing resource identified by the Request-URI and other existing resources.
[LOCK][lock]                            | no   | no         | Used to take out a lock of any access type and to refresh an existing lock.
[MERGE][merge]                          | no   | yes        | Performs the logical merge of a specified version (the "merge source") into a specified version-controlled resource (the "merge target").
[MKACTIVITY][mkactivity]                | no   | yes        | Creates a new activity resource.
[MKCALENDAR][mkcalendar]                | no   | yes        | Creates a new calendar collection resource.
[MKCOL][mkcol]                          | no   | yes        | Creates a new collection resource at the location specified by the Request-URI.
[MKREDIRECTREF][mkredirectref]          | no   | yes        | Requests the creation of a redirect reference resource.
[MKWORKSPACE][mkworkspace]              | no   | yes        | Creates a new workspace resource.
[MOVE][move]                            | no   | yes        | On a non-collection resource is the logical equivalent of a copy (COPY), followed by consistency maintenance processing, followed by a delete of the source, where all three actions are performed in a single operation.
[OPTIONS][options]                      | yes  | yes        | Requests information about the communication options available for the target resource, at either the origin server or an intervening intermediary.
[ORDERPATCH][orderpatch]                | no   | yes        | Is used to change the ordering semantics of a collection, to change the order of the collection's members in the ordering, or both.
[PATCH][patch]                          | no   | no         | That a set of changes described in the request entity be applied to the resource identified by the Request-URI.
[POST][post]                            | no   | no         | Requests that the target resource process the representation enclosed in the request according to the resource's own specific semantics.
[PRI][pri]                              | yes  | yes        | Used when an HTTP/1.1 server or intermediary attempts to parse an HTTP/2 connection preface.
[PROPFIND][propfind]                    | yes  | yes        | Retrieves properties defined on the resource identified by the Request-URI, if the resource does not have any internal members, or on the resource identified by the Request-URI and potentially its member resources, if the resource is a collection that has internal member URLs.
[PROPPATCH][proppatch]                  | no   | yes        | Processes instructions specified in the request body to set and/or remove properties defined on the resource identified by the Request-URI.
[PUT][put]                              | no   | yes        | Requests that the state of the target resource be created or replaced with the state defined by the representation enclosed in the request message payload.
[REBIND][rebind]                        | no   | yes        | Removes a binding to a resource from a collection, and adds a binding to that resource into the collection identified by the Request-URI.
[REPORT][report]                        | yes  | yes        | An extensible mechanism for obtaining information about a resource.
[SEARCH][search]                        | yes  | yes        | Initiate a server-side search.
[TRACE][trace]                          | yes  | yes        | Requests a remote, application-level loop-back of the request message.
[UNBIND][unbind]                        | no   | yes        | Modifies the collection identified by the Request-URI by removing the binding identified by the segment specified in the UNBIND body.
[UNCHECKOUT][uncheckout]                | no   | yes        | can be applied to a checked-out version-controlled resource to cancel the CHECKOUT and restore the pre-CHECKOUT state of the version-controlled resource.
[UNLINK][unlink]                        | no   | yes        | Removes one or more Link relationships from the existing resource identified by the Request-URI.
[UNLOCK][unlock]                        | no   | yes        | Removes the lock identified by the lock token in the Lock-Token request header.
[UPDATE][update]                        | no   | yes        | Modifies the content and dead properties of a checked-in version-controlled resource (the "update target") to be those of a specified version (the "update source") from the version history of that version-controlled resource.
[UPDTEREDIRECTREF][updateredirectref]   | no   | yes        | Requests the update of a redirect reference resource.
[VERSION-CONTROL][version-control]      | no   | yes        | Can be used to create a version-controlled resource at the request-URL.

[acl]:               http://tools.ietf.org/html/rfc3744#section-8.1
[baseline-control]:  http://tools.ietf.org/html/rfc3253#section-12.6
[bind]:              http://tools.ietf.org/html/rfc5842#section-4
[checkin-1]:         http://tools.ietf.org/html/rfc3253#section-4.4
[checkin-2]:         http://tools.ietf.org/html/rfc3253#section-9.4
[connect]:           http://tools.ietf.org/html/rfc7231#section-4.3.6
[copy]:              http://tools.ietf.org/html/rfc4918#section-9.8
[delete]:            http://tools.ietf.org/html/rfc7231#section-4.3.5
[get]:               http://tools.ietf.org/html/rfc7231#section-4.3.1
[head]:              http://tools.ietf.org/html/rfc7231#section-4.3.2
[label]:             http://tools.ietf.org/html/rfc3253#section-8.2
[link]:              http://tools.ietf.org/html/rfc2068#section-19.6.1.2
[lock]:              http://tools.ietf.org/html/rfc4918#section-9.10
[merge]:             http://tools.ietf.org/html/rfc3253#section-11.2
[mkactivity]:        http://tools.ietf.org/html/rfc3253#section-13.5
[mkcalendar]:        http://tools.ietf.org/html/rfc4791#section-5.3.1
[mkcol]:             http://tools.ietf.org/html/rfc4918#section-9.3
[mkredirectref]:     http://tools.ietf.org/html/rfc4437#section-6
[mkworkspace]:       http://tools.ietf.org/html/rfc3253#section-6.3
[move]:              http://tools.ietf.org/html/rfc4918#section-9.9
[options]:           http://tools.ietf.org/html/rfc7231#section-4.3.7
[orderpatch]:        http://tools.ietf.org/html/rfc3648#section-7
[patch]:             http://tools.ietf.org/html/rfc5789#section-2
[post]:              http://tools.ietf.org/html/rfc7231#section-4.3.3
[pri]:               http://tools.ietf.org/html/draft-ietf-httpbis-http2-17#section-3.5
[propfind]:          http://tools.ietf.org/html/rfc4918#section-9.1
[proppatch]:         http://tools.ietf.org/html/rfc4918#section-9.2
[put]:               http://tools.ietf.org/html/rfc7231#section-4.3.4
[rebind]:            http://tools.ietf.org/html/rfc5842#section-6
[report]:            http://tools.ietf.org/html/rfc3253#section-3.6
[search]:            http://tools.ietf.org/html/rfc5323#section-2
[trace]:             http://tools.ietf.org/html/rfc7231#section-4.3.8
[unbind]:            http://tools.ietf.org/html/rfc5842#section-5
[uncheckout]:        http://tools.ietf.org/html/rfc3253#section-4.5
[unlink]:            http://tools.ietf.org/html/rfc2068#section-19.6.1.3
[unlock]:            http://tools.ietf.org/html/rfc4918#section-9.11
[update]:            http://tools.ietf.org/html/rfc3253#section-7.1
[updateredirectref]: http://tools.ietf.org/html/rfc4437#section-7 
[version-control]:   http://tools.ietf.org/html/rfc3253#section-3.5
