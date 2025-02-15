---
title: Constant tauri::http::header::PROXY_AUTHENTICATE
sidebar_label: constant.PROXY_AUTHENTICATE
custom_edit_url: null
---

  # Constant tauri::http&#x3A;:header::PROXY_AUTHENTICATE,

```rs
pub const PROXY_AUTHENTICATE: HeaderName;
```

Expand description

Defines the authentication method that should be used to gain access to a proxy.

Unlike `www-authenticate`, the `proxy-authenticate` header field applies only to the next outbound client on the response chain. This is because only the client that chose a given proxy is likely to have the credentials necessary for authentication. However, when multiple proxies are used within the same administrative domain, such as office and regional caching proxies within a large corporate network, it is common for credentials to be generated by the user agent and passed through the hierarchy until consumed. Hence, in such a configuration, it will appear as if Proxy-Authenticate is being forwarded because each proxy will send the same challenge set.

The `proxy-authenticate` header is sent along with a `407 Proxy Authentication Required`.
  