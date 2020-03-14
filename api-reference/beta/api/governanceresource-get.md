---
title: 获取 governanceResource
description: 检索 governanceResource 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identitiy-platform
ms.openlocfilehash: 235b4cdfffd5573af5a5470ee5687e4a17ec42c6
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639875"
---
# <a name="get-governanceresource"></a><span data-ttu-id="544b5-103">获取 governanceResource</span><span class="sxs-lookup"><span data-stu-id="544b5-103">Get governanceResource</span></span>

<span data-ttu-id="544b5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="544b5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="544b5-105">检索[governanceResource](../resources/governanceresource.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="544b5-105">Retrieve the properties and relationships of a [governanceResource](../resources/governanceresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="544b5-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="544b5-106">Permissions</span></span>
<span data-ttu-id="544b5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="544b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="544b5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="544b5-109">Permission type</span></span>      | <span data-ttu-id="544b5-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="544b5-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="544b5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="544b5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="544b5-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="544b5-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="544b5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="544b5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="544b5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="544b5-114">Not supported.</span></span>    |
|<span data-ttu-id="544b5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="544b5-115">Application</span></span> | <span data-ttu-id="544b5-116">PrivilegedAccess。 AzureResources</span><span class="sxs-lookup"><span data-stu-id="544b5-116">PrivilegedAccess.Read.AzureResources</span></span> |

<span data-ttu-id="544b5-117">除了权限范围之外，此 API 还要求请求者具有对资源的至少一个角色分配。</span><span class="sxs-lookup"><span data-stu-id="544b5-117">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="544b5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="544b5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="544b5-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="544b5-119">Optional query parameters</span></span>
<span data-ttu-id="544b5-120">此方法**仅**支持`$select`和`$expand` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="544b5-120">This method **only** supports  `$select` and `$expand` [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="544b5-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="544b5-121">Request headers</span></span>
| <span data-ttu-id="544b5-122">名称</span><span class="sxs-lookup"><span data-stu-id="544b5-122">Name</span></span>      |<span data-ttu-id="544b5-123">说明</span><span class="sxs-lookup"><span data-stu-id="544b5-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="544b5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="544b5-124">Authorization</span></span>  | <span data-ttu-id="544b5-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="544b5-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="544b5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="544b5-126">Request body</span></span>
<span data-ttu-id="544b5-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="544b5-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="544b5-128">响应</span><span class="sxs-lookup"><span data-stu-id="544b5-128">Response</span></span>
<span data-ttu-id="544b5-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[governanceResource](../resources/governanceresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="544b5-129">If successful, this method returns a `200 OK` response code and [governanceResource](../resources/governanceresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="544b5-130">示例</span><span class="sxs-lookup"><span data-stu-id="544b5-130">Example</span></span>
<span data-ttu-id="544b5-131">本示例演示如何获取订阅 Wingtip 玩具-生产（e5e7d29d-5465-45ac-885f-4716a5ee74b5）的详细信息。</span><span class="sxs-lookup"><span data-stu-id="544b5-131">This example shows how to get the details of the subscription Wingtip Toys - Prod (e5e7d29d-5465-45ac-885f-4716a5ee74b5).</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="544b5-132">请求</span><span class="sxs-lookup"><span data-stu-id="544b5-132">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5
```
##### <a name="response"></a><span data-ttu-id="544b5-133">响应</span><span class="sxs-lookup"><span data-stu-id="544b5-133">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 459

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceResources/$entity",
    "id": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",
    "type": "subscription",
    "displayName": "Wingtip Toys - Prod",
    "status": "Active",
    "registeredDateTime": "2018-04-05T22:30:37.13Z",
    "registeredRoot": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",    
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
