---
title: Microsoft Graph 安全 API 错误响应
description: 返回使用标准 HTTP 206 部分内容状态代码和传递通过警告标头中 Microsoft Graph 中的 Microsoft Graph 安全 API 的错误。
ms.openlocfilehash: 35af0a1ed4c4bf7f6e1afb36039f812ab59f64dd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011436"
---
# <a name="microsoft-graph-security-api-error-responses"></a><span data-ttu-id="31640-103">Microsoft Graph 安全 API 错误响应</span><span class="sxs-lookup"><span data-stu-id="31640-103">Microsoft Graph Security API error responses</span></span>

<span data-ttu-id="31640-104">返回使用标准 HTTP 206 部分内容状态代码和传递通过警告标头中 Microsoft Graph 中的 Microsoft Graph 安全 API 的错误。</span><span class="sxs-lookup"><span data-stu-id="31640-104">Errors in the Microsoft Graph Security API in Microsoft Graph are returned using standard HTTP 206 Partial Content status code and are delivered by way of a warning header.</span></span>

<span data-ttu-id="31640-105">Microsoft Graph 安全 API 为从所有数据提供程序接收多个响应联合的服务。</span><span class="sxs-lookup"><span data-stu-id="31640-105">The Microsoft Graph Security API is a federated service that receives multiple responses from all data providers.</span></span> <span data-ttu-id="31640-106">由 Microsoft Graph 安全 API 收到 HTTP 错误时，它将发送回警告标头采用以下格式：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="31640-106">When an HTTP error is received by the Microsoft Graph Security API, it will send back a warning header in the following format: <!-- { "blockType": "ignored" } --></span></span>

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

<span data-ttu-id="31640-107">一个数据提供程序返回之外的 2xx 或 404 错误代码时，此警告标头将只发送回客户端。</span><span class="sxs-lookup"><span data-stu-id="31640-107">This warning header is only sent back to clients when one of the data providers returns an error code other than 2xx or 404.</span></span> <span data-ttu-id="31640-108">例如：</span><span class="sxs-lookup"><span data-stu-id="31640-108">For example:</span></span>

- <span data-ttu-id="31640-109">如果未授予对资源的访问权限，则可能会返回 HttpStatusCode.Forbidden (403)。</span><span class="sxs-lookup"><span data-stu-id="31640-109">HttpStatusCode.Forbidden (403) might be returned if the access to the resource is not granted.</span></span>
- <span data-ttu-id="31640-110">如果提供程序超时，警告标头中返回 HttpStatusCode.GatewayTimeout (504)。</span><span class="sxs-lookup"><span data-stu-id="31640-110">If a provider times out, HttpStatusCode.GatewayTimeout (504) is returned in the warning header.</span></span>
- <span data-ttu-id="31640-111">如果内部的提供程序错误发生的情况，警告标头中使用 HttpStatusCode.InternalServerError (500)。</span><span class="sxs-lookup"><span data-stu-id="31640-111">If an internal provider error happens, HttpStatusCode.InternalServerError (500) is used in the warning header.</span></span>

<span data-ttu-id="31640-112">如果数据提供程序返回 2xx 或 404，它不显示警告标头因为需要以获得成功进行这些代码时，或者在未分别找到数据。</span><span class="sxs-lookup"><span data-stu-id="31640-112">If a data provider returns 2xx or 404, it’s not shown in the warning header because these codes are expected for success or when data is not found respectively.</span></span> <span data-ttu-id="31640-113">在联合系统中，如多次数据到一个或多个，但不是所有的提供程序仅已知预期 404 找不到。</span><span class="sxs-lookup"><span data-stu-id="31640-113">In a federated system, a 404 not found is expected as many times the data is only known to one or several, but not all, providers.</span></span>

## <a name="example"></a><span data-ttu-id="31640-114">示例</span><span class="sxs-lookup"><span data-stu-id="31640-114">Example</span></span>

<span data-ttu-id="31640-115">用户询问的`security/alerts/{alert_id}`。</span><span class="sxs-lookup"><span data-stu-id="31640-115">A user asks for `security/alerts/{alert_id}`.</span></span>

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

<span data-ttu-id="31640-116">由于 404 和 200 是预期的条件，警告头包含以下信息：</span><span class="sxs-lookup"><span data-stu-id="31640-116">Because both 404 and 200 are expected conditions, the warning header contains the following:</span></span> 

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> <span data-ttu-id="31640-117">**注意：** 每个 HTTP 标头是子项，集合，以便用户可以枚举警告标头，并检查所有项目。</span><span class="sxs-lookup"><span data-stu-id="31640-117">**Note:** Each HTTP header is a collection of subitems, so users can enumerate the Warning header and check all items.</span></span>

## <a name="see-also"></a><span data-ttu-id="31640-118">另请参阅</span><span class="sxs-lookup"><span data-stu-id="31640-118">See also</span></span>

<span data-ttu-id="31640-119">如果您遇到授权时遇到问题，请参阅我们的[博客文章](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/Authorization-and-Microsoft-Graph-Security-API/m-p/184376#M2)。</span><span class="sxs-lookup"><span data-stu-id="31640-119">If you’re having trouble with authorization, see our [blog post](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/Authorization-and-Microsoft-Graph-Security-API/m-p/184376#M2).</span></span>
