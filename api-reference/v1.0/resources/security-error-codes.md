# <a name="security-api-error-responses"></a>安全性 API 错误响应

Microsoft Graph 安全性 API 中的错误使用标准 HTTP 状态代码返回，并通过警告标头提供。

安全性 API 是一种联合服务，它接收来自所有数据提供程序的多个响应。 当安全性 API 收到 HTTP 错误时，它将以下列格式发回警告标头： <!-- { "blockType": "ignored" } -->

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

当其中一个数据提供程序返回 2xx 或 404 以外的错误代码时，此警告标头仅发送回客户端。 例如：

- 如果未授予对资源的访问权限，则可能会返回 HttpStatusCode.Forbidden (403)。
- 如果提供程序超时，则在警告标题中返回 HttpStatusCode.GatewayTimeout (504)。
- 如果发生内部提供程序错误，则在警告标头中使用 HttpStatusCode.InternalServerError (500)。

如果数据提供程序返回 2xx 或 404，则它不会显示在警告标头中，因为这些代码预计会成功或分别找不到数据。 在联合系统中，预期未找到 404 的数据仅为一个或多个（但不是所有）提供程序所知的数据。

## <a name="example"></a>示例

用户要求 `security/alerts/{alert_id}`。

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

由于 404 和 200 都是预期条件，因此警告标头包含以下内容： 

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/29000",    (usual timeout limit is set at 29 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> **注意：** 每个 HTTP 标头都是子项集合，因此用户可以枚举警告标头并检查所有项。

## <a name="see-also"></a>另请参阅

如果您在授权方面遇到问题，请参阅我们的[博客文章](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/Authorization-and-Microsoft-Graph-Security-API/m-p/184376#M2)。
