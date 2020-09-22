---
title: Microsoft Graph 安全性 API 错误响应
description: Microsoft Graph 安全性 API 中的错误使用标准的 HTTP 206 部分内容状态代码返回，并通过警告标头进行传递。
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: conceptualPageType
ms.openlocfilehash: c36cf3be4cf24a2831918acd994a36bbcfc9e489
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988924"
---
# <a name="microsoft-graph-security-api-error-responses"></a><span data-ttu-id="6c1e9-103">Microsoft Graph 安全性 API 错误响应</span><span class="sxs-lookup"><span data-stu-id="6c1e9-103">Microsoft Graph Security API error responses</span></span>

<span data-ttu-id="6c1e9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c1e9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6c1e9-105">Microsoft Graph 安全性 API 中的错误使用标准的 HTTP 206 部分内容状态代码返回，并通过警告标头进行传递。</span><span class="sxs-lookup"><span data-stu-id="6c1e9-105">Errors in the Microsoft Graph Security API are returned using the standard HTTP 206 Partial Content status code and are delivered via a warning header.</span></span>

## <a name="errors"></a><span data-ttu-id="6c1e9-106">错误</span><span class="sxs-lookup"><span data-stu-id="6c1e9-106">Errors</span></span>

<span data-ttu-id="6c1e9-107">Microsoft Graph 安全性 API 是一种联合服务，可接收来自所有数据提供程序的多个响应。</span><span class="sxs-lookup"><span data-stu-id="6c1e9-107">The Microsoft Graph Security API is a federated service that receives multiple responses from all data providers.</span></span> <span data-ttu-id="6c1e9-108">当 Microsoft Graph 安全性 API 收到 HTTP 错误时，它将以以下格式返回一个警告标头：</span><span class="sxs-lookup"><span data-stu-id="6c1e9-108">When an HTTP error is received by the Microsoft Graph Security API, it will send back a warning header in the following format:</span></span>
<!-- { "blockType": "ignored" } -->

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

<span data-ttu-id="6c1e9-109">仅当其中一个数据提供程序返回了2xx 或404之外的错误代码时，此警告标头才会发送回客户端。</span><span class="sxs-lookup"><span data-stu-id="6c1e9-109">This warning header is only sent back to clients when one of the data providers returns an error code other than 2xx or 404.</span></span> <span data-ttu-id="6c1e9-110">例如：</span><span class="sxs-lookup"><span data-stu-id="6c1e9-110">For example:</span></span>

- <span data-ttu-id="6c1e9-111">如果未授予对资源的访问权限，则可能会返回 HttpStatusCode (403) 。</span><span class="sxs-lookup"><span data-stu-id="6c1e9-111">HttpStatusCode.Forbidden (403) might be returned if the access to the resource is not granted.</span></span>
- <span data-ttu-id="6c1e9-112">如果提供程序超时，则在警告标头中返回 HttpStatusCode (504) 。</span><span class="sxs-lookup"><span data-stu-id="6c1e9-112">If a provider times out, HttpStatusCode.GatewayTimeout (504) is returned in the warning header.</span></span>
- <span data-ttu-id="6c1e9-113">如果发生内部提供程序错误，则在警告标头中使用 InternalServerError (500) HttpStatusCode。</span><span class="sxs-lookup"><span data-stu-id="6c1e9-113">If an internal provider error happens, HttpStatusCode.InternalServerError (500) is used in the warning header.</span></span>

<span data-ttu-id="6c1e9-114">如果数据提供程序返回2xx 或404，则它不会显示在警告标头中，因为这些代码是成功的，或者是在不分别找到数据时。</span><span class="sxs-lookup"><span data-stu-id="6c1e9-114">If a data provider returns 2xx or 404, it’s not shown in the warning header because these codes are expected for success or when data is not found respectively.</span></span> <span data-ttu-id="6c1e9-115">在联合系统中，未找到404的次数预期数据只对一个或多个（但不是所有）提供程序已知。</span><span class="sxs-lookup"><span data-stu-id="6c1e9-115">In a federated system, a 404 not found is expected as many times the data is only known to one or several, but not all, providers.</span></span>

## <a name="example"></a><span data-ttu-id="6c1e9-116">示例</span><span class="sxs-lookup"><span data-stu-id="6c1e9-116">Example</span></span>

<span data-ttu-id="6c1e9-117">用户请求 `security/alerts/{alert_id}` 。</span><span class="sxs-lookup"><span data-stu-id="6c1e9-117">A user asks for `security/alerts/{alert_id}`.</span></span>

```
Provider 1: 404 (provider does not have a record of this alert ID)
Provider 2: 504 (provider timed out)
Provider 3: 200 (success)
Provider 4: 403 (customer has not licensed this provider)
```

<span data-ttu-id="6c1e9-118">由于404和200都是预期条件，因此警告标头包含以下内容：</span><span class="sxs-lookup"><span data-stu-id="6c1e9-118">Because both 404 and 200 are expected conditions, the warning header contains the following:</span></span>

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> <span data-ttu-id="6c1e9-119">**注意：** 每个 HTTP 标头都是一个子项集合，因此用户可以枚举警告标头并选中所有项目。</span><span class="sxs-lookup"><span data-stu-id="6c1e9-119">**Note:** Each HTTP header is a collection of subitems, so users can enumerate the Warning header and check all items.</span></span>

## <a name="threat-indicator-bulk-action-errors"></a><span data-ttu-id="6c1e9-120">威胁指示器批量操作错误</span><span class="sxs-lookup"><span data-stu-id="6c1e9-120">Threat indicator bulk action errors</span></span>

<span data-ttu-id="6c1e9-121"> (创建、更新、删除) 的批量操作可生成两个不同的潜在错误代码：</span><span class="sxs-lookup"><span data-stu-id="6c1e9-121">Bulk actions (create, update, delete) can generate two different potential error codes:</span></span>

- <span data-ttu-id="6c1e9-122">400错误代码指示提供的正文在序列化过程中出现错误。</span><span class="sxs-lookup"><span data-stu-id="6c1e9-122">A 400 error code indicates that the body provided had an error during serialization.</span></span>
- <span data-ttu-id="6c1e9-123">206错误代码指示在将一个或多个批量操作与提供程序联合时失败。</span><span class="sxs-lookup"><span data-stu-id="6c1e9-123">A 206 error code indicates that one or more of the bulk actions failed when it was federated out to its provider.</span></span> <span data-ttu-id="6c1e9-124">响应将包含各个提供商针对每个威胁情报指标的成功/错误数据。</span><span class="sxs-lookup"><span data-stu-id="6c1e9-124">The response will contain success/error data from the individual providers for each threat intelligence indicator.</span></span> <span data-ttu-id="6c1e9-125">与 [警报](/graph/api/resources/security-api-overview?view=graph-rest-1.0#alerts)不同，所有潜在的错误信息将包含在 [tiIndicator](/graph/api/resources/security-api-overview?view=graph-rest-beta#threat-indicators-preview) 批量操作的响应正文中。</span><span class="sxs-lookup"><span data-stu-id="6c1e9-125">Unlike [alerts](/graph/api/resources/security-api-overview?view=graph-rest-1.0#alerts), all potential error information will be contained within the body of the response for [tiIndicator](/graph/api/resources/security-api-overview?view=graph-rest-beta#threat-indicators-preview) bulk actions.</span></span>

## <a name="constraints"></a><span data-ttu-id="6c1e9-126">约束</span><span class="sxs-lookup"><span data-stu-id="6c1e9-126">Constraints</span></span>

<span data-ttu-id="6c1e9-127">`$top`OData 查询参数限制为1000个警报。</span><span class="sxs-lookup"><span data-stu-id="6c1e9-127">The `$top` OData query parameter has a limit of 1000 alerts.</span></span> <span data-ttu-id="6c1e9-128">建议你在第一个 GET 查询中仅包括 `$top`，而不包括 `$skip`。</span><span class="sxs-lookup"><span data-stu-id="6c1e9-128">We recommend that you include only `$top` and not `$skip` in your first GET query.</span></span> <span data-ttu-id="6c1e9-129">可使用 `@odata.nextLink` 进行分页。</span><span class="sxs-lookup"><span data-stu-id="6c1e9-129">You can use `@odata.nextLink` for pagination.</span></span> <span data-ttu-id="6c1e9-130">如果需要使用 `$skip`，它具有 500 个警报的限制。</span><span class="sxs-lookup"><span data-stu-id="6c1e9-130">If you need to use `$skip`, it has a limit of 500 alerts.</span></span> <span data-ttu-id="6c1e9-131">例如，`/security/alerts?$top=10&$skip=500` 将返回 `200 OK` 响应代码，但 `/security/alerts?$top=10&$skip=501` 将返回 `400 Bad Request` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6c1e9-131">For example, `/security/alerts?$top=10&$skip=500` will return a `200 OK` response code, but `/security/alerts?$top=10&$skip=501` will return a `400 Bad Request` response code.</span></span> <span data-ttu-id="6c1e9-132">有关详细信息，请参阅 [Microsoft Graph 安全性 API 错误响应](../resources/security-error-codes.md)。</span><span class="sxs-lookup"><span data-stu-id="6c1e9-132">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

<span data-ttu-id="6c1e9-133">此限制的解决方法是将 `$filter` OData 查询参数与 `eventDateTime` Microsoft GRAPH 安全 API 中的 alert 实体结合使用， `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` 并将 dateTime 值替换为最后一个 (1500th) 警报。</span><span class="sxs-lookup"><span data-stu-id="6c1e9-133">A workaround for this limit is to use the `$filter` OData query parameter with the `eventDateTime` of the alert entity from the Microsoft Graph Security API, using `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` and replacing the dateTime value with the last (1500th) alert.</span></span> <span data-ttu-id="6c1e9-134">您还可以为设置区域 `eventDateTime` ; 例如， `alerts?$filter=eventDateTime **gt** 2018-11-**11**T00:00:00.000Z&eventDateTime **lt** 2018-11-**12**T00:00:00.000Z` 。</span><span class="sxs-lookup"><span data-stu-id="6c1e9-134">You can also set a range for the `eventDateTime`; for example, `alerts?$filter=eventDateTime **gt** 2018-11-**11**T00:00:00.000Z&eventDateTime **lt** 2018-11-**12**T00:00:00.000Z`.</span></span>

## <a name="see-also"></a><span data-ttu-id="6c1e9-135">另请参阅</span><span class="sxs-lookup"><span data-stu-id="6c1e9-135">See also</span></span>

<span data-ttu-id="6c1e9-136">如果您在使用授权时遇到问题，请参阅 [授权和 Microsoft Graph 安全性 API](/graph/security-authorization)。</span><span class="sxs-lookup"><span data-stu-id="6c1e9-136">If you’re having trouble with authorization, see [Authorization and the Microsoft Graph Security API](/graph/security-authorization).</span></span>


