---
title: 获取 governanceResource
description: 检索的属性和 governanceResource 对象的关系。
ms.openlocfilehash: d871dbe91b82cebc01a8c282c0afdfbd8701c8f0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041925"
---
# <a name="get-governanceresource"></a><span data-ttu-id="940b3-103">获取 governanceResource</span><span class="sxs-lookup"><span data-stu-id="940b3-103">Get governanceResource</span></span>

> <span data-ttu-id="940b3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="940b3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="940b3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="940b3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="940b3-106">检索的属性和[governanceResource](../resources/governanceresource.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="940b3-106">Retrieve the properties and relationships of a [governanceResource](../resources/governanceresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="940b3-107">权限</span><span class="sxs-lookup"><span data-stu-id="940b3-107">Permissions</span></span>
<span data-ttu-id="940b3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="940b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="940b3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="940b3-110">Permission type</span></span>      | <span data-ttu-id="940b3-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="940b3-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="940b3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="940b3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="940b3-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="940b3-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="940b3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="940b3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="940b3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="940b3-115">Not supported.</span></span>    |
|<span data-ttu-id="940b3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="940b3-116">Application</span></span> | <span data-ttu-id="940b3-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="940b3-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="940b3-118">除了权限范围，此 API 要求具有至少一个角色分配对资源的请求程序。</span><span class="sxs-lookup"><span data-stu-id="940b3-118">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="940b3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="940b3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="940b3-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="940b3-120">Optional query parameters</span></span>
<span data-ttu-id="940b3-121">此方法**仅**支持`$select`和`$expand` [OData 查询参数](/graph/query-parameters)，以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="940b3-121">This method **only** supports  `$select` and `$expand` [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="940b3-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="940b3-122">Request headers</span></span>
| <span data-ttu-id="940b3-123">名称</span><span class="sxs-lookup"><span data-stu-id="940b3-123">Name</span></span>      |<span data-ttu-id="940b3-124">说明</span><span class="sxs-lookup"><span data-stu-id="940b3-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="940b3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="940b3-125">Authorization</span></span>  | <span data-ttu-id="940b3-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="940b3-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="940b3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="940b3-127">Request body</span></span>
<span data-ttu-id="940b3-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="940b3-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="940b3-129">响应</span><span class="sxs-lookup"><span data-stu-id="940b3-129">Response</span></span>
<span data-ttu-id="940b3-130">如果成功，此方法返回`200 OK`响应正文中的响应代码和[governanceResource](../resources/governanceresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="940b3-130">If successful, this method returns a `200 OK` response code and [governanceResource](../resources/governanceresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="940b3-131">示例</span><span class="sxs-lookup"><span data-stu-id="940b3-131">Example</span></span>
<span data-ttu-id="940b3-132">本示例演示如何获取订阅 Wingtip Toys-prod 移 (e5e7d29d-5465-45ac-885f-4716a5ee74b5) 的详细信息。</span><span class="sxs-lookup"><span data-stu-id="940b3-132">This example shows how to get the details of the subscription Wingtip Toys - Prod (e5e7d29d-5465-45ac-885f-4716a5ee74b5).</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="940b3-133">请求</span><span class="sxs-lookup"><span data-stu-id="940b3-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5
```
##### <a name="response"></a><span data-ttu-id="940b3-134">响应</span><span class="sxs-lookup"><span data-stu-id="940b3-134">Response</span></span>
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
    "onboardDateTime": "2018-04-05T22:30:37.13Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
