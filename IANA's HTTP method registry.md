# IANA's HTTP method registry <sup>[[source]](http://www.iana.org/assignments/http-methods/http-methods.xhtml)</sup>

**Safe** methods don’t modify resources.
**Idempotent** methods can be called many times without different outcomes.

Method name                           | Safe | Idempotent
-----------                           | ---- | ----------
[ACL][acl]                            | no   | yes
[BASELINE-CONTROL][baseline-control]  | no   | yes
[BIND][bind]                          | no   | yes
CHECKIN[¹][checkin-1][²][checkin-2]   | no   | yes
[CONNECT][connect]                    | no   | no
[COPY][copy]                          | no   | yes
[DELETE][delete]                      | no   | yes
[GET][get]                            | yes  | yes
[HEAD][head]                          | yes  | yes
[LABEL][label]                        | no   | yes
[LINK][link]                          | no   | yes
[LOCK][lock]                          | no   | no
[MERGE][merge]                        | no   | yes
[MKACTIVITY][mkactivity]              | no   | yes
[MKCALENDAR][mkcalendar]              | no   | yes
[MKCOL][mkcol]                        | no   | yes
[MKREDIRECTREF][mkredirectref]        | no   | yes
[MKWORKSPACE][mkworkspace]            | no   | yes
[MOVE][move]                          | no   | yes
[OPTIONS][options]                    | yes  | yes
[ORDERPATCH][orderpatch]              | no   | yes
[PATCH][patch]                        | no   | no
[POST][post]                          | no   | no
[PRI][pri]                            | yes  | yes
[PROPFIND][propfind]                  | yes  | yes
[PROPPATCH][proppatch]                | no   | yes 
[PUT][put]                            | no   | yes
[REBIND][rebind]                      | no   | yes
[REPORT][report]                      | yes  | yes
[SEARCH][search]                      | yes  | yes
[TRACE][trace]                        | yes  | yes
[UNBIND][unbind]                      | no   | yes
[UNCHECKOUT][uncheckout]              | no   | yes
[UNLINK][unlink]                      | no   | yes
[UNLOCK][unlock]                      | no   | yes
[UPDATE][update]                      | no   | yes
[UPDTEREDIRECTREF][updateredirectref] | no   | yes
[VERSION-CONTROL][version-control]    | no   | yes

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