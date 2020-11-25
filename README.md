# bigip-irule-samples
Some usefull iRule samples. The samples are provided as is, and should be used with caution :).

# irule_clientcert_acl
This irule is a "stub" example on how to implement client cert validation on a BIG-IP LTM virtual server.

Features:
* Validate client certificate issuing CA (relies on client-ssl profile on the virtual server)
* Validate client certificate CN
* Validate client certificate serial
* Logging to syslog

If all client certificate checks are ok, the irule responds with a HTTP 200 Ok. The HTTP response can be replaced with whatever suits your requirements.

Prerequisites are a working virtual server with a http profile and a client-ssl profile. The client-ssl profile should be configured with client cert require and the issuing CA to validate against.
