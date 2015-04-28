# RFC 7231 HTTP status codes <sup>[[source]](http://tools.ietf.org/html/rfc7231)</sup>

Code       | Reason-Phrase                 | Description
----       | ----                          | -----------
[100][100] | Continue                      | The initial part of a request has been received and has not yet been rejected by the server.
[101][101] | Switching Protocols           | The server understands and is willing to comply with the client's request, via the Upgrade header field, for a change in the application protocol being used on this connection.
[200][200] | OK                            | The request has succeeded.
[201][201] | Created                       | The request has been fulfilled and has resulted in one or more new resources being created.
[202][202] | Accepted                      | The request has been accepted for processing, but the processing has not been completed.
[203][203] | Non-Authoritative Information | The request was successful but the enclosed payload has been modified from that of the origin server's 200 (OK) response by a transforming proxy.
[204][204] | No Content                    | The server has successfully fulfilled the request and that there is no additional content to send in the response payload body.
[205][205] | Reset Content                 | The server has fulfilled the request and desires that the user agent reset the "document view", which caused the request to be sent, to its original state as received from the origin server.
[206][206] | Partial Content               | The server is successfully fulfilling a range request for the target resource by transferring one or more parts of the selected representation that correspond to the satisfiable ranges found in the request's Range header field.
[300][300] | Multiple Choices              | The target resource has more than one representation, each with its own more specific identifier, and information about the alternatives is being provided so that the user (or user agent) can select a preferred representation by redirecting its request to one or more of those identifiers.
[301][301] | Moved Permanently             | The target resource has been assigned a new permanent URI and any future references to this resource ought to use one of the enclosed URIs.
[302][302] | Found                         | The target resource resides temporarily under a different URI.
[303][303] | See Other                     | The server is redirecting the user agent to a different resource, as indicated by a URI in the Location header field, which is intended to provide an indirect response to the original request.
[304][304] | Not Modified                  | A conditional GET or HEAD request has been received and would have resulted in a 200 (OK) response if it were not for the fact that the condition evaluated to false.
[305][305] | Use Proxy                     | *deprecated*
[307][307] | Temporary Redirect            | The target resource resides temporarily under a different URI and the user agent MUST NOT change the request method if it performs an automatic redirection to that URI.
[400][400] | Bad Request                   | The server cannot or will not process the request due to something that is perceived to be a client error (e.g., malformed request syntax, invalid request message framing, or deceptive request routing).
[401][401] | Unauthorized                  | The request has not been applied because it lacks valid authentication credentials for the target resource.
[402][402] | Payment Required              | *reserved for future use*
[403][403] | Forbidden                     | The server understood the request but refuses to authorize it.
[404][404] | Not Found                     | The origin server did not find a current representation for the target resource or is not willing to disclose that one exists.
[405][405] | Method Not Allowed            | The method received in the request-line is known by the origin server but not supported by the target resource.
[406][406] | Not Acceptable                | The target resource does not have a current representation that would be acceptable to the user agent, according to the proactive negotiation header fields received in the request, and the server is unwilling to supply a default representation.
[407][407] | Proxy Authentication Required | Similar to 401 (Unauthorized), but it indicates that the client needs to authenticate itself in order to use a proxy.
[408][408] | Request Timeout               | The server did not receive a complete request message within the time that it was prepared to wait.
[409][409] | Conflict                      | The request could not be completed due to a conflict with the current state of the target resource.
[410][410] | Gone                          | Access to the target resource is no longer available at the origin server and that this condition is likely to be permanent.
[411][411] | Length Required               | The server refuses to accept the request without a defined Content-Length.
[412][412] | Precondition Failed           | One or more conditions given in the request header fields evaluated to false when tested on the server.
[413][413] | Payload Too Large             | The server is refusing to process a request because the request payload is larger than the server is willing or able to process.
[414][414] | URI Too Long                  | The server is refusing to service the request because the request target is longer than the server is willing to interpret.
[415][415] | Unsupported Media Type        | The origin server is refusing to service the request because the payload is in a format not supported by this method on the target resource.
[416][416] | Range Not Satisfiable         | None of the ranges in the request's Range header field overlap the current extent of the selected resource or that the set of ranges requested has been rejected due to invalid ranges or an excessive request of small or overlapping ranges.
[417][417] | Expectation Failed            | The expectation given in the request's Expect header field could not be met by at least one of the inbound servers.
[426][426] | Upgrade Required              | The server refuses to perform the request using the current protocol but might be willing to do so after the client upgrades to a different protocol.
[500][500] | Internal Server Error         | The server encountered an unexpected condition that prevented it from fulfilling the request.
[501][501] | Not Implemented               | The server does not support the functionality required to fulfill the request.
[502][502] | Bad Gateway                   | The server, while acting as a gateway or proxy, received an invalid response from an inbound server it accessed while attempting to fulfill the request.
[503][503] | Service Unavailable           | The server is currently unable to handle the request due to a temporary overload or scheduled maintenance, which will likely be alleviated after some delay.
[504][504] | Gateway Timeout               | The server, while acting as a gateway or proxy, did not receive a timely response from an upstream server it needed to access in order to complete the request.
[505][505] | HTTP Version Not Supported    | The server does not support, or refuses to support, the majorversion of HTTP that was used in the request message.

[100]: http://tools.ietf.org/html/rfc7231#section-6.2.1
[101]: http://tools.ietf.org/html/rfc7231#section-6.2.2
[200]: http://tools.ietf.org/html/rfc7231#section-6.3.1
[201]: http://tools.ietf.org/html/rfc7231#section-6.3.2
[202]: http://tools.ietf.org/html/rfc7231#section-6.3.3
[203]: http://tools.ietf.org/html/rfc7231#section-6.3.4
[204]: http://tools.ietf.org/html/rfc7231#section-6.3.5
[205]: http://tools.ietf.org/html/rfc7231#section-6.3.6
[206]: http://tools.ietf.org/html/rfc7233#section-4.1
[300]: http://tools.ietf.org/html/rfc7231#section-6.4.1
[301]: http://tools.ietf.org/html/rfc7231#section-6.4.2
[302]: http://tools.ietf.org/html/rfc7231#section-6.4.3
[303]: http://tools.ietf.org/html/rfc7231#section-6.4.4
[304]: http://tools.ietf.org/html/rfc7232#section-4.1
[305]: http://tools.ietf.org/html/rfc7231#section-6.4.5
[307]: http://tools.ietf.org/html/rfc7231#section-6.4.7
[400]: http://tools.ietf.org/html/rfc7231#section-6.5.1
[401]: http://tools.ietf.org/html/rfc7235#section-3.1
[402]: http://tools.ietf.org/html/rfc7231#section-6.5.2
[403]: http://tools.ietf.org/html/rfc7231#section-6.5.3
[404]: http://tools.ietf.org/html/rfc7231#section-6.5.4
[405]: http://tools.ietf.org/html/rfc7231#section-6.5.5
[406]: http://tools.ietf.org/html/rfc7231#section-6.5.6
[407]: http://tools.ietf.org/html/rfc7235#section-3.2
[408]: http://tools.ietf.org/html/rfc7231#section-6.5.7
[409]: http://tools.ietf.org/html/rfc7231#section-6.5.8
[410]: http://tools.ietf.org/html/rfc7231#section-6.5.9
[411]: http://tools.ietf.org/html/rfc7231#section-6.5.10
[412]: http://tools.ietf.org/html/rfc7232#section-4.2
[413]: http://tools.ietf.org/html/rfc7231#section-6.5.11
[414]: http://tools.ietf.org/html/rfc7231#section-6.5.12
[415]: http://tools.ietf.org/html/rfc7231#section-6.5.13
[416]: http://tools.ietf.org/html/rfc7233#section-4.4
[417]: http://tools.ietf.org/html/rfc7231#section-6.5.14
[426]: http://tools.ietf.org/html/rfc7231#section-6.5.15
[500]: http://tools.ietf.org/html/rfc7231#section-6.6.1
[501]: http://tools.ietf.org/html/rfc7231#section-6.6.2
[502]: http://tools.ietf.org/html/rfc7231#section-6.6.3
[503]: http://tools.ietf.org/html/rfc7231#section-6.6.4
[504]: http://tools.ietf.org/html/rfc7231#section-6.6.5
[505]: http://tools.ietf.org/html/rfc7231#section-6.6.6
