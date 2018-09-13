# <a name="security-api-error-responses"></a><span data-ttu-id="ff39a-101">安全性 API 错误响应</span><span class="sxs-lookup"><span data-stu-id="ff39a-101">Security API error responses</span></span>

<span data-ttu-id="ff39a-102">Microsoft Graph 安全性 API 中的错误使用标准 HTTP 状态代码返回，并通过警告标头提供。</span><span class="sxs-lookup"><span data-stu-id="ff39a-102">Errors in the security API in Microsoft Graph are returned using standard HTTP status codes and are delivered by way of a warning header.</span></span>

<span data-ttu-id="ff39a-103">安全性 API 是一种联合服务，它接收来自所有数据提供程序的多个响应。</span><span class="sxs-lookup"><span data-stu-id="ff39a-103">The security API is a federated service that receives multiple responses from all data providers.</span></span> <span data-ttu-id="ff39a-104">当安全性 API 收到 HTTP 错误时，它将以下列格式发回警告标头： <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="ff39a-104">When an HTTP error is received by the security API, it will send back a warning header in the following format: <!-- { "blockType": "ignored" } --></span></span>

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

<span data-ttu-id="ff39a-105">当其中一个数据提供程序返回 2xx 或 404 以外的错误代码时，此警告标头仅发送回客户端。</span><span class="sxs-lookup"><span data-stu-id="ff39a-105">This warning header is only sent back to clients when one of the data providers returns an error code other than 2xx or 404.</span></span> <span data-ttu-id="ff39a-106">例如：</span><span class="sxs-lookup"><span data-stu-id="ff39a-106">For example:</span></span>

- <span data-ttu-id="ff39a-107">如果未授予对资源的访问权限，则可能会返回 HttpStatusCode.Forbidden (403)。</span><span class="sxs-lookup"><span data-stu-id="ff39a-107">HttpStatusCode.Forbidden (403) might be returned if the access to the resource is not granted.</span></span>
- <span data-ttu-id="ff39a-108">如果提供程序超时，则在警告标题中返回 HttpStatusCode.GatewayTimeout (504)。</span><span class="sxs-lookup"><span data-stu-id="ff39a-108">If a provider times out, HttpStatusCode.GatewayTimeout (504) is returned in the warning header.</span></span>
- <span data-ttu-id="ff39a-109">如果发生内部提供程序错误，则在警告标头中使用 HttpStatusCode.InternalServerError (500)。</span><span class="sxs-lookup"><span data-stu-id="ff39a-109">If an internal provider error happens, HttpStatusCode.InternalServerError (500) is used in the warning header.</span></span>

<span data-ttu-id="ff39a-110">如果数据提供程序返回 2xx 或 404，则它不会显示在警告标头中，因为这些代码预计会成功或分别找不到数据。</span><span class="sxs-lookup"><span data-stu-id="ff39a-110">If a data provider returns 2xx or 404, it’s not shown in the warning header because these codes are expected for success or when data is not found respectively.</span></span> <span data-ttu-id="ff39a-111">在联合系统中，预期未找到 404 的数据仅为一个或多个（但不是所有）提供程序所知的数据。</span><span class="sxs-lookup"><span data-stu-id="ff39a-111">In a federated system, a 404 not found is expected as many times the data is only known to one or several, but not all, providers.</span></span>

## <a name="example"></a><span data-ttu-id="ff39a-112">示例</span><span class="sxs-lookup"><span data-stu-id="ff39a-112">Example</span></span>

<span data-ttu-id="ff39a-113">用户要求 `security/alerts/{alert_id}`。</span><span class="sxs-lookup"><span data-stu-id="ff39a-113">A user asks for `security/alerts/{alert_id}`.</span></span>

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

<span data-ttu-id="ff39a-114">由于 404 和 200 都是预期条件，因此警告标头包含以下内容：</span><span class="sxs-lookup"><span data-stu-id="ff39a-114">Because both 404 and 200 are expected conditions, the warning header contains the following:</span></span> 

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/29000",    (usual timeout limit is set at 29 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> <span data-ttu-id="ff39a-115">**注意：** 每个 HTTP 标头都是子项集合，因此用户可以枚举警告标头并检查所有项。</span><span class="sxs-lookup"><span data-stu-id="ff39a-115">**Note:** Each HTTP header is a collection of subitems, so users can enumerate the Warning header and check all items.</span></span>

## <a name="see-also"></a><span data-ttu-id="ff39a-116">另请参阅</span><span class="sxs-lookup"><span data-stu-id="ff39a-116">See also</span></span>

<span data-ttu-id="ff39a-117">如果您在授权方面遇到问题，请参阅我们的[博客文章](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/Authorization-and-Microsoft-Graph-Security-API/m-p/184376#M2)。</span><span class="sxs-lookup"><span data-stu-id="ff39a-117">If you’re having trouble with authorization, see our [blog post](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/Authorization-and-Microsoft-Graph-Security-API/m-p/184376#M2).</span></span>
