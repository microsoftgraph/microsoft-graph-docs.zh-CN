---
title: Microsoft Graph 安全性 API 错误响应
description: Microsoft Graph 安全性 API 中的错误使用标准的 HTTP 206 部分内容状态代码返回, 并通过警告标头进行传递。
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: conceptualPageType
ms.openlocfilehash: 2d77a0f21623a98e4041b845e92a23c7574a415d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034466"
---
# <a name="microsoft-graph-security-api-error-responses"></a><span data-ttu-id="79299-103">Microsoft Graph 安全性 API 错误响应</span><span class="sxs-lookup"><span data-stu-id="79299-103">Microsoft Graph Security API error responses</span></span>

<span data-ttu-id="79299-104">Microsoft Graph 安全性 API 中的错误使用标准的 HTTP 206 部分内容状态代码返回, 并通过警告标头进行传递。</span><span class="sxs-lookup"><span data-stu-id="79299-104">Errors in the Microsoft Graph Security API are returned using the standard HTTP 206 Partial Content status code and are delivered via a warning header.</span></span>

## <a name="errors"></a><span data-ttu-id="79299-105">错误</span><span class="sxs-lookup"><span data-stu-id="79299-105">Errors</span></span>

<span data-ttu-id="79299-106">Microsoft Graph 安全性 API 是一种联合服务, 可接收来自所有数据提供程序的多个响应。</span><span class="sxs-lookup"><span data-stu-id="79299-106">The Microsoft Graph Security API is a federated service that receives multiple responses from all data providers.</span></span> <span data-ttu-id="79299-107">当 Microsoft Graph 安全性 API 收到 HTTP 错误时, 它将以以下格式返回一个警告标头:</span><span class="sxs-lookup"><span data-stu-id="79299-107">When an HTTP error is received by the Microsoft Graph Security API, it will send back a warning header in the following format:</span></span>
<!-- { "blockType": "ignored" } -->

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

<span data-ttu-id="79299-108">仅当其中一个数据提供程序返回了2xx 或404之外的错误代码时, 此警告标头才会发送回客户端。</span><span class="sxs-lookup"><span data-stu-id="79299-108">This warning header is only sent back to clients when one of the data providers returns an error code other than 2xx or 404.</span></span> <span data-ttu-id="79299-109">例如：</span><span class="sxs-lookup"><span data-stu-id="79299-109">For example:</span></span>

- <span data-ttu-id="79299-110">如果未授予对资源的访问权限, 则可能会返回 HttpStatusCode (403)。</span><span class="sxs-lookup"><span data-stu-id="79299-110">HttpStatusCode.Forbidden (403) might be returned if the access to the resource is not granted.</span></span>
- <span data-ttu-id="79299-111">如果提供程序超时, 则在警告标头中返回 HttpStatusCode GatewayTimeout (504)。</span><span class="sxs-lookup"><span data-stu-id="79299-111">If a provider times out, HttpStatusCode.GatewayTimeout (504) is returned in the warning header.</span></span>
- <span data-ttu-id="79299-112">如果发生内部提供程序错误, 则在警告标头中使用 InternalServerError (500) HttpStatusCode。</span><span class="sxs-lookup"><span data-stu-id="79299-112">If an internal provider error happens, HttpStatusCode.InternalServerError (500) is used in the warning header.</span></span>

<span data-ttu-id="79299-113">如果数据提供程序返回2xx 或 404, 则它不会显示在警告标头中, 因为这些代码是成功的, 或者是在不分别找到数据时。</span><span class="sxs-lookup"><span data-stu-id="79299-113">If a data provider returns 2xx or 404, it’s not shown in the warning header because these codes are expected for success or when data is not found respectively.</span></span> <span data-ttu-id="79299-114">在联合系统中, 未找到404的次数预期数据只对一个或多个 (但不是所有) 提供程序已知。</span><span class="sxs-lookup"><span data-stu-id="79299-114">In a federated system, a 404 not found is expected as many times the data is only known to one or several, but not all, providers.</span></span>

## <a name="example"></a><span data-ttu-id="79299-115">示例</span><span class="sxs-lookup"><span data-stu-id="79299-115">Example</span></span>

<span data-ttu-id="79299-116">用户请求`security/alerts/{alert_id}`。</span><span class="sxs-lookup"><span data-stu-id="79299-116">A user asks for `security/alerts/{alert_id}`.</span></span>

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

<span data-ttu-id="79299-117">由于404和200都是预期条件, 因此警告标头包含以下内容:</span><span class="sxs-lookup"><span data-stu-id="79299-117">Because both 404 and 200 are expected conditions, the warning header contains the following:</span></span>

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> <span data-ttu-id="79299-118">**注意:** 每个 HTTP 标头都是一个子项集合, 因此用户可以枚举警告标头并选中所有项目。</span><span class="sxs-lookup"><span data-stu-id="79299-118">**Note:** Each HTTP header is a collection of subitems, so users can enumerate the Warning header and check all items.</span></span>

## <a name="constraints"></a><span data-ttu-id="79299-119">约束</span><span class="sxs-lookup"><span data-stu-id="79299-119">Constraints</span></span>

<span data-ttu-id="79299-120">Odata 查询参数的限制为1000个警报, 而`$top`  +  `$skip` odata 查询参数的组合不能超过6000个警报。 `$top`</span><span class="sxs-lookup"><span data-stu-id="79299-120">The `$top` OData query parameter has a limit of 1000 alerts, and a combination of `$top` + `$skip` OData query parameters cannot exceed 6000 alerts.</span></span> <span data-ttu-id="79299-121">例如，`/security/alerts?$top=10&$skip=5990` 将返回 `200 OK` 响应代码，但 `/security/alerts?$top=10&$skip=5991` 将返回 `400 Bad Request` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="79299-121">For example, `/security/alerts?$top=10&$skip=5990` will return a `200 OK` response code, but `/security/alerts?$top=10&$skip=5991` will return a `400 Bad Request` response code.</span></span>

<span data-ttu-id="79299-122">此限制的解决方法是将`$filter` OData 查询参数与 Microsoft GRAPH 安全 API 中`eventDateTime`的 alert 实体结合使用, `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}`并将 dateTime 值替换为最后的 (6000th) 警报。</span><span class="sxs-lookup"><span data-stu-id="79299-122">A work-around for this limit is to use the `$filter` OData query parameter with the `eventDateTime` of the alert entity from the Microsoft Graph Security API, using `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` and replacing the dateTime value with the last (6000th) alert.</span></span> <span data-ttu-id="79299-123">您还可以为设置区域`eventDateTime`;例如,*警报？ $filter = eventDateTime **gt** 2018-11-**11**T00:00: 00.000 z&eventDateTime **lt** 2018-11-**12**T00:00: 00.000 z*</span><span class="sxs-lookup"><span data-stu-id="79299-123">You can also set a range for the `eventDateTime`; for example, *alerts?$filter=eventDateTime **gt** 2018-11-**11**T00:00:00.000Z&eventDateTime **lt** 2018-11-**12**T00:00:00.000Z*</span></span>

## <a name="see-also"></a><span data-ttu-id="79299-124">另请参阅</span><span class="sxs-lookup"><span data-stu-id="79299-124">See also</span></span>

<span data-ttu-id="79299-125">如果您在使用授权时遇到问题, 请参阅[授权和 Microsoft Graph 安全性 API](/graph/security-authorization)。</span><span class="sxs-lookup"><span data-stu-id="79299-125">If you’re having trouble with authorization, see [Authorization and the Microsoft Graph Security API](/graph/security-authorization).</span></span>
