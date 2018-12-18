---
title: Microsoft Graph 安全 API 错误响应
description: 返回使用标准 HTTP 206 部分内容状态代码和传递通过警告标头中 Microsoft Graph 安全 API 的错误。
author: Preetikr
ms.openlocfilehash: 6685d69f202696e33422d9bd3a877cba02fd10dd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334417"
---
# <a name="microsoft-graph-security-api-error-responses"></a><span data-ttu-id="3322a-103">Microsoft Graph 安全 API 错误响应</span><span class="sxs-lookup"><span data-stu-id="3322a-103">Microsoft Graph Security API error responses</span></span>

<span data-ttu-id="3322a-104">返回使用标准 HTTP 206 部分内容状态代码和传递通过警告标头中 Microsoft Graph 安全 API 的错误。</span><span class="sxs-lookup"><span data-stu-id="3322a-104">Errors in the Microsoft Graph Security API are returned using the standard HTTP 206 Partial Content status code and are delivered via a warning header.</span></span>

## <a name="errors"></a><span data-ttu-id="3322a-105">错误</span><span class="sxs-lookup"><span data-stu-id="3322a-105">Errors</span></span>

<span data-ttu-id="3322a-106">Microsoft Graph 安全 API 为从所有数据提供程序接收多个响应联合的服务。</span><span class="sxs-lookup"><span data-stu-id="3322a-106">The Microsoft Graph Security API is a federated service that receives multiple responses from all data providers.</span></span> <span data-ttu-id="3322a-107">由 Microsoft Graph 安全 API 收到 HTTP 错误时，它将发送回警告标头采用以下格式：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="3322a-107">When an HTTP error is received by the Microsoft Graph Security API, it will send back a warning header in the following format: <!-- { "blockType": "ignored" } --></span></span>

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

<span data-ttu-id="3322a-108">一个数据提供程序返回之外的 2xx 或 404 错误代码时，此警告标头将只发送回客户端。</span><span class="sxs-lookup"><span data-stu-id="3322a-108">This warning header is only sent back to clients when one of the data providers returns an error code other than 2xx or 404.</span></span> <span data-ttu-id="3322a-109">例如：</span><span class="sxs-lookup"><span data-stu-id="3322a-109">For example:</span></span>

- <span data-ttu-id="3322a-110">如果未授予对资源的访问权限，则可能会返回 HttpStatusCode.Forbidden (403)。</span><span class="sxs-lookup"><span data-stu-id="3322a-110">HttpStatusCode.Forbidden (403) might be returned if the access to the resource is not granted.</span></span>
- <span data-ttu-id="3322a-111">如果提供程序超时，警告标头中返回 HttpStatusCode.GatewayTimeout (504)。</span><span class="sxs-lookup"><span data-stu-id="3322a-111">If a provider times out, HttpStatusCode.GatewayTimeout (504) is returned in the warning header.</span></span>
- <span data-ttu-id="3322a-112">如果内部的提供程序错误发生的情况，警告标头中使用 HttpStatusCode.InternalServerError (500)。</span><span class="sxs-lookup"><span data-stu-id="3322a-112">If an internal provider error happens, HttpStatusCode.InternalServerError (500) is used in the warning header.</span></span>

<span data-ttu-id="3322a-113">如果数据提供程序返回 2xx 或 404，它不显示警告标头因为需要以获得成功进行这些代码时，或者在未分别找到数据。</span><span class="sxs-lookup"><span data-stu-id="3322a-113">If a data provider returns 2xx or 404, it’s not shown in the warning header because these codes are expected for success or when data is not found respectively.</span></span> <span data-ttu-id="3322a-114">在联合系统中，如多次数据到一个或多个，但不是所有的提供程序仅已知预期 404 找不到。</span><span class="sxs-lookup"><span data-stu-id="3322a-114">In a federated system, a 404 not found is expected as many times the data is only known to one or several, but not all, providers.</span></span>

## <a name="example"></a><span data-ttu-id="3322a-115">示例</span><span class="sxs-lookup"><span data-stu-id="3322a-115">Example</span></span>

<span data-ttu-id="3322a-116">用户询问的`security/alerts/{alert_id}`。</span><span class="sxs-lookup"><span data-stu-id="3322a-116">A user asks for `security/alerts/{alert_id}`.</span></span>

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

<span data-ttu-id="3322a-117">由于 404 和 200 是预期的条件，警告头包含以下信息：</span><span class="sxs-lookup"><span data-stu-id="3322a-117">Because both 404 and 200 are expected conditions, the warning header contains the following:</span></span>

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> <span data-ttu-id="3322a-118">**注意：** 每个 HTTP 标头是子项，集合，以便用户可以枚举警告标头，并检查所有项目。</span><span class="sxs-lookup"><span data-stu-id="3322a-118">**Note:** Each HTTP header is a collection of subitems, so users can enumerate the Warning header and check all items.</span></span>

## <a name="constraints"></a><span data-ttu-id="3322a-119">约束</span><span class="sxs-lookup"><span data-stu-id="3322a-119">Constraints</span></span>

<span data-ttu-id="3322a-120">`$top` OData 查询参数的限制为 1000年警报和组合`$top`  +  `$skip`参数不能超过 6000 通知的 OData 查询。</span><span class="sxs-lookup"><span data-stu-id="3322a-120">The `$top` OData query parameter has a limit of 1000 alerts, and a combination of `$top` + `$skip` OData query parameters cannot exceed 6000 alerts.</span></span> <span data-ttu-id="3322a-121">例如，`/security/alerts?$top=10&$skip=5990`会返回`200 OK`响应代码，但`/security/alerts?$top=10&$skip=5991`将返回`400 Bad Request`响应代码。</span><span class="sxs-lookup"><span data-stu-id="3322a-121">For example, `/security/alerts?$top=10&$skip=5990` will return a `200 OK` response code, but `/security/alerts?$top=10&$skip=5991` will return a `400 Bad Request` response code.</span></span>

<span data-ttu-id="3322a-122">解决此限制的方法是使用`$filter`OData 查询参数`eventDateTime`从 Microsoft Graph 安全 API，警报实体的使用`?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}`和 dateTime 值替换 (6000th) 的最后一个通知。</span><span class="sxs-lookup"><span data-stu-id="3322a-122">A work-around for this limit is to use the `$filter` OData query parameter with the `eventDateTime` of the alert entity from the Microsoft Graph Security API, using `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` and replacing the dateTime value with the last (6000th) alert.</span></span> <span data-ttu-id="3322a-123">您还可以设置范围`eventDateTime`;例如， *alerts?$ filter = eventDateTime **gt** 2018-11-**11**T00:00:00.000Z = eventDateTime **lt** 2018-11-**12**T00:00:00.000Z*</span><span class="sxs-lookup"><span data-stu-id="3322a-123">You can also set a range for the `eventDateTime`; for example, *alerts?$filter=eventDateTime **gt** 2018-11-**11**T00:00:00.000Z&eventDateTime **lt** 2018-11-**12**T00:00:00.000Z*</span></span>

## <a name="see-also"></a><span data-ttu-id="3322a-124">另请参阅</span><span class="sxs-lookup"><span data-stu-id="3322a-124">See also</span></span>

<span data-ttu-id="3322a-125">如果您遇到授权时遇到问题，请参阅[Authorization and Microsoft Graph 安全 API](/graph/security-authorization)。</span><span class="sxs-lookup"><span data-stu-id="3322a-125">If you’re having trouble with authorization, see [Authorization and the Microsoft Graph Security API](/graph/security-authorization).</span></span>
