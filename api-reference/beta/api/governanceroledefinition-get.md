---
title: 获取 governanceRoleDefinition
description: 检索 governanceRoleDefinition 的属性和关系。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 26295521d7d8558d902f1e1f6fecef3ed27a1a5d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42420897"
---
# <a name="get-governanceroledefinition"></a><span data-ttu-id="0ed80-103">获取 governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="0ed80-103">Get governanceRoleDefinition</span></span>

<span data-ttu-id="0ed80-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0ed80-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ed80-105">检索[governanceRoleDefinition](../resources/governanceroledefinition.md)的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0ed80-105">Retrieve the properties and relationships of a [governanceRoleDefinition](../resources/governanceroledefinition.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0ed80-106">权限</span><span class="sxs-lookup"><span data-stu-id="0ed80-106">Permissions</span></span>
<span data-ttu-id="0ed80-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ed80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ed80-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ed80-109">Permission type</span></span>      | <span data-ttu-id="0ed80-110">权限</span><span class="sxs-lookup"><span data-stu-id="0ed80-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ed80-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ed80-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0ed80-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="0ed80-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="0ed80-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ed80-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ed80-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ed80-114">Not supported.</span></span>    |
|<span data-ttu-id="0ed80-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ed80-115">Application</span></span> | <span data-ttu-id="0ed80-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ed80-116">Not supported.</span></span> |

<span data-ttu-id="0ed80-117">除了权限范围之外，此 API 还要求请求者在资源上至少具有一个角色分配， [governanceRoleDefinition](../resources/governanceroledefinition.md)属于该资源。</span><span class="sxs-lookup"><span data-stu-id="0ed80-117">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleDefinition](../resources/governanceroledefinition.md) belongs to.</span></span>

## <a name="http-request"></a><span data-ttu-id="0ed80-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ed80-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions/{id}
GET /privilegedAccess/azureResources/roleDefinitions/{id}?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0ed80-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0ed80-119">Optional query parameters</span></span>
<span data-ttu-id="0ed80-120">此方法**不**支持[OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0ed80-120">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ed80-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ed80-121">Request headers</span></span>
| <span data-ttu-id="0ed80-122">名称</span><span class="sxs-lookup"><span data-stu-id="0ed80-122">Name</span></span>      |<span data-ttu-id="0ed80-123">说明</span><span class="sxs-lookup"><span data-stu-id="0ed80-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0ed80-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ed80-124">Authorization</span></span>  | <span data-ttu-id="0ed80-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0ed80-125">Bearer {code}</span></span>|


## <a name="request-body"></a><span data-ttu-id="0ed80-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ed80-126">Request body</span></span>
<span data-ttu-id="0ed80-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0ed80-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0ed80-128">响应</span><span class="sxs-lookup"><span data-stu-id="0ed80-128">Response</span></span>
<span data-ttu-id="0ed80-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[governanceRoleDefinition](../resources/governanceroledefinition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0ed80-129">If successful, this method returns a `200 OK` response code and [governanceRoleDefinition](../resources/governanceroledefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0ed80-130">示例</span><span class="sxs-lookup"><span data-stu-id="0ed80-130">Example</span></span>
<span data-ttu-id="0ed80-131">本示例演示如何在订阅 Wingtip 玩具-生产中获取角色定义 DNS 区域参与者的详细信息。</span><span class="sxs-lookup"><span data-stu-id="0ed80-131">This example shows how to get details of role definition DNS Zone Contributor in the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinition"
}-->
##### <a name="request"></a><span data-ttu-id="0ed80-132">请求</span><span class="sxs-lookup"><span data-stu-id="0ed80-132">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions/00efc9e0-1b96-4e9a-99a3-a3df0735cf88
```
##### <a name="response"></a><span data-ttu-id="0ed80-133">响应</span><span class="sxs-lookup"><span data-stu-id="0ed80-133">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleDefinition"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 174

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleDefinitions/$entity",
    "id": "00efc9e0-1b96-4e9a-99a3-a3df0735cf88",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/befefa01-2a29-4197-83a8-272ff33ce314",
    "templateId": "befefa01-2a29-4197-83a8-272ff33ce314",
    "displayName": "DNS Zone Contributor"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
