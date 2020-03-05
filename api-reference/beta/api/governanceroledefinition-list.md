---
title: 列出 governanceRoleDefinitions
description: 获取资源的 governanceRoleDefinitions 集合。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 3b8d45a3d4f5f89ed35fd2defaf733d2d03af097
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42420890"
---
# <a name="list-governanceroledefinitions"></a><span data-ttu-id="c6d1f-103">列出 governanceRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="c6d1f-103">List governanceRoleDefinitions</span></span>

<span data-ttu-id="c6d1f-104">命名空间： microsoft. graph[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="c6d1f-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="c6d1f-105">获取资源的[governanceRoleDefinitions](../resources/governanceroledefinition.md)集合。</span><span class="sxs-lookup"><span data-stu-id="c6d1f-105">Get a collection of [governanceRoleDefinitions](../resources/governanceroledefinition.md) on a resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6d1f-106">权限</span><span class="sxs-lookup"><span data-stu-id="c6d1f-106">Permissions</span></span>
<span data-ttu-id="c6d1f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c6d1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6d1f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c6d1f-109">Permission type</span></span>      | <span data-ttu-id="c6d1f-110">权限</span><span class="sxs-lookup"><span data-stu-id="c6d1f-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6d1f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c6d1f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c6d1f-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="c6d1f-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="c6d1f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c6d1f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6d1f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6d1f-114">Not supported.</span></span>    |
|<span data-ttu-id="c6d1f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c6d1f-115">Application</span></span> | <span data-ttu-id="c6d1f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6d1f-116">Not supported.</span></span> |

<span data-ttu-id="c6d1f-117">除了权限范围之外，此 API 还要求请求者具有对资源的至少一个角色分配。</span><span class="sxs-lookup"><span data-stu-id="c6d1f-117">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="c6d1f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c6d1f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions
GET /privilegedAccess/azureResources/roleDefinitions?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c6d1f-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c6d1f-119">Optional query parameters</span></span>
<span data-ttu-id="c6d1f-120">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c6d1f-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c6d1f-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c6d1f-121">Request headers</span></span>
| <span data-ttu-id="c6d1f-122">名称</span><span class="sxs-lookup"><span data-stu-id="c6d1f-122">Name</span></span>      |<span data-ttu-id="c6d1f-123">说明</span><span class="sxs-lookup"><span data-stu-id="c6d1f-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c6d1f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6d1f-124">Authorization</span></span>  | <span data-ttu-id="c6d1f-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c6d1f-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6d1f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c6d1f-126">Request body</span></span>
<span data-ttu-id="c6d1f-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c6d1f-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c6d1f-128">响应</span><span class="sxs-lookup"><span data-stu-id="c6d1f-128">Response</span></span>
<span data-ttu-id="c6d1f-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[governanceRoleDefinition](../resources/governanceroledefinition.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="c6d1f-129">If successful, this method returns a `200 OK` response code and collection of [governanceRoleDefinition](../resources/governanceroledefinition.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c6d1f-130">示例</span><span class="sxs-lookup"><span data-stu-id="c6d1f-130">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinitions"
}-->
<span data-ttu-id="c6d1f-131">本示例演示如何获取订阅 Wingtip 玩具-生产的所有角色定义。</span><span class="sxs-lookup"><span data-stu-id="c6d1f-131">This example shows how to get all role definitions of the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="c6d1f-132">请求</span><span class="sxs-lookup"><span data-stu-id="c6d1f-132">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions  
```
##### <a name="response"></a><span data-ttu-id="c6d1f-133">响应</span><span class="sxs-lookup"><span data-stu-id="c6d1f-133">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleDefinition",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 21906

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleDefinitions",
    "value": [
        {
            "id": "00efc9e0-1b96-4e9a-99a3-a3df0735cf88",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/befefa01-2a29-4197-83a8-272ff33ce314",
            "templateId": "befefa01-2a29-4197-83a8-272ff33ce314",
            "displayName": "DNS Zone Contributor"
        },
        {
            "id": "051f7264-a992-429a-b345-90415af9f917",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/c12c1c16-33a1-487b-954d-41c89c60f349",
            "templateId": "c12c1c16-33a1-487b-954d-41c89c60f349",
            "displayName": "Reader and Data Access"
        },
        {
            "id": "0789c03d-445d-40ab-aed3-d110a98146c7",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/5d28c62d-5b37-4476-8438-e587778df237",
            "templateId": "5d28c62d-5b37-4476-8438-e587778df237",
            "displayName": "New Relic APM Account Contributor"
        },
  ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List governanceRoleDefinitions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
