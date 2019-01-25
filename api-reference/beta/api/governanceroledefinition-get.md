---
title: 获取 governanceRoleDefinition
description: 检索的属性和 governanceRoleDefinition 的关系。
localization_priority: Normal
ms.openlocfilehash: e6a057816a8e07a355941f272325c30078327ab9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511924"
---
# <a name="get-governanceroledefinition"></a><span data-ttu-id="3b6d2-103">获取 governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="3b6d2-103">Get governanceRoleDefinition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b6d2-104">检索的属性和[governanceRoleDefinition](../resources/governanceroledefinition.md)的关系。</span><span class="sxs-lookup"><span data-stu-id="3b6d2-104">Retrieve the properties and relationships of a [governanceRoleDefinition](../resources/governanceroledefinition.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3b6d2-105">权限</span><span class="sxs-lookup"><span data-stu-id="3b6d2-105">Permissions</span></span>
<span data-ttu-id="3b6d2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3b6d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b6d2-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3b6d2-108">Permission type</span></span>      | <span data-ttu-id="3b6d2-109">权限</span><span class="sxs-lookup"><span data-stu-id="3b6d2-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b6d2-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3b6d2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3b6d2-111">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="3b6d2-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="3b6d2-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3b6d2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b6d2-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b6d2-113">Not supported.</span></span>    |
|<span data-ttu-id="3b6d2-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3b6d2-114">Application</span></span> | <span data-ttu-id="3b6d2-115">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="3b6d2-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="3b6d2-116">除了权限范围，此 API 要求的请求程序上的资源， [governanceRoleDefinition](../resources/governanceroledefinition.md)属于必须至少一个角色分配。</span><span class="sxs-lookup"><span data-stu-id="3b6d2-116">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleDefinition](../resources/governanceroledefinition.md) belongs to.</span></span>

## <a name="http-request"></a><span data-ttu-id="3b6d2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3b6d2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions/{id}
GET /privilegedAccess/azureResources/roleDefinitions/{id}?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3b6d2-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3b6d2-118">Optional query parameters</span></span>
<span data-ttu-id="3b6d2-119">此方法执行**不**支持的[OData 查询参数](/graph/query-parameters)以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="3b6d2-119">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3b6d2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3b6d2-120">Request headers</span></span>
| <span data-ttu-id="3b6d2-121">名称</span><span class="sxs-lookup"><span data-stu-id="3b6d2-121">Name</span></span>      |<span data-ttu-id="3b6d2-122">说明</span><span class="sxs-lookup"><span data-stu-id="3b6d2-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3b6d2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b6d2-123">Authorization</span></span>  | <span data-ttu-id="3b6d2-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3b6d2-124">Bearer {code}</span></span>|


## <a name="request-body"></a><span data-ttu-id="3b6d2-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="3b6d2-125">Request body</span></span>
<span data-ttu-id="3b6d2-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3b6d2-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3b6d2-127">响应</span><span class="sxs-lookup"><span data-stu-id="3b6d2-127">Response</span></span>
<span data-ttu-id="3b6d2-128">如果成功，此方法返回`200 OK`响应正文中的响应代码和[governanceRoleDefinition](../resources/governanceroledefinition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3b6d2-128">If successful, this method returns a `200 OK` response code and [governanceRoleDefinition](../resources/governanceroledefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3b6d2-129">示例</span><span class="sxs-lookup"><span data-stu-id="3b6d2-129">Example</span></span>
<span data-ttu-id="3b6d2-130">本示例演示如何获取 Wingtip Toys-prod 移订阅中的角色定义 DNS 区域参与者的详细信息。</span><span class="sxs-lookup"><span data-stu-id="3b6d2-130">This example shows how to get details of role definition DNS Zone Contributor in the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinition"
}-->
##### <a name="request"></a><span data-ttu-id="3b6d2-131">请求</span><span class="sxs-lookup"><span data-stu-id="3b6d2-131">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions/00efc9e0-1b96-4e9a-99a3-a3df0735cf88
```
##### <a name="response"></a><span data-ttu-id="3b6d2-132">响应</span><span class="sxs-lookup"><span data-stu-id="3b6d2-132">Response</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroledefinition-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
