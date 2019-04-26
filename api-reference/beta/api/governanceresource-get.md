---
title: 获取 governanceResource
description: 检索 governanceResource 对象的属性和关系。
localization_priority: Normal
ms.openlocfilehash: 30c5c5404e11ba5394c306c8d6196cdf58954d25
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329621"
---
# <a name="get-governanceresource"></a><span data-ttu-id="9bda7-103">获取 governanceResource</span><span class="sxs-lookup"><span data-stu-id="9bda7-103">Get governanceResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bda7-104">检索[governanceResource](../resources/governanceresource.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9bda7-104">Retrieve the properties and relationships of a [governanceResource](../resources/governanceresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9bda7-105">权限</span><span class="sxs-lookup"><span data-stu-id="9bda7-105">Permissions</span></span>
<span data-ttu-id="9bda7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9bda7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bda7-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9bda7-108">Permission type</span></span>      | <span data-ttu-id="9bda7-109">权限</span><span class="sxs-lookup"><span data-stu-id="9bda7-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9bda7-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9bda7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9bda7-111">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="9bda7-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="9bda7-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9bda7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9bda7-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9bda7-113">Not supported.</span></span>    |
|<span data-ttu-id="9bda7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9bda7-114">Application</span></span> | <span data-ttu-id="9bda7-115">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="9bda7-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="9bda7-116">除了权限范围之外, 此 API 还要求请求者具有对资源的至少一个角色分配。</span><span class="sxs-lookup"><span data-stu-id="9bda7-116">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="9bda7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9bda7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9bda7-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9bda7-118">Optional query parameters</span></span>
<span data-ttu-id="9bda7-119">此方法**仅**支持`$select`和`$expand` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9bda7-119">This method **only** supports  `$select` and `$expand` [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9bda7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9bda7-120">Request headers</span></span>
| <span data-ttu-id="9bda7-121">名称</span><span class="sxs-lookup"><span data-stu-id="9bda7-121">Name</span></span>      |<span data-ttu-id="9bda7-122">说明</span><span class="sxs-lookup"><span data-stu-id="9bda7-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9bda7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bda7-123">Authorization</span></span>  | <span data-ttu-id="9bda7-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9bda7-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bda7-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9bda7-125">Request body</span></span>
<span data-ttu-id="9bda7-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9bda7-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9bda7-127">响应</span><span class="sxs-lookup"><span data-stu-id="9bda7-127">Response</span></span>
<span data-ttu-id="9bda7-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[governanceResource](../resources/governanceresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9bda7-128">If successful, this method returns a `200 OK` response code and [governanceResource](../resources/governanceresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bda7-129">示例</span><span class="sxs-lookup"><span data-stu-id="9bda7-129">Example</span></span>
<span data-ttu-id="9bda7-130">本示例演示如何获取订阅 Wingtip 玩具-生产 (e5e7d29d-5465-45ac-885f-4716a5ee74b5) 的详细信息。</span><span class="sxs-lookup"><span data-stu-id="9bda7-130">This example shows how to get the details of the subscription Wingtip Toys - Prod (e5e7d29d-5465-45ac-885f-4716a5ee74b5).</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="9bda7-131">请求</span><span class="sxs-lookup"><span data-stu-id="9bda7-131">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5
```
##### <a name="response"></a><span data-ttu-id="9bda7-132">响应</span><span class="sxs-lookup"><span data-stu-id="9bda7-132">Response</span></span>
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
