---
title: 列表 governanceRoleDefinitions
description: 获取对资源的 governanceRoleDefinitions 集合。
localization_priority: Normal
ms.openlocfilehash: 0e03a75446723743cc43eef63c42dd0f39c86126
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525197"
---
# <a name="list-governanceroledefinitions"></a><span data-ttu-id="c9b48-103">列表 governanceRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="c9b48-103">List governanceRoleDefinitions</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9b48-104">获取对资源的[governanceRoleDefinitions](../resources/governanceroledefinition.md)集合。</span><span class="sxs-lookup"><span data-stu-id="c9b48-104">Get a collection of [governanceRoleDefinitions](../resources/governanceroledefinition.md) on a resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9b48-105">权限</span><span class="sxs-lookup"><span data-stu-id="c9b48-105">Permissions</span></span>
<span data-ttu-id="c9b48-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c9b48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9b48-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c9b48-108">Permission type</span></span>      | <span data-ttu-id="c9b48-109">权限</span><span class="sxs-lookup"><span data-stu-id="c9b48-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9b48-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c9b48-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c9b48-111">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="c9b48-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="c9b48-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c9b48-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9b48-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c9b48-113">Not supported.</span></span>    |
|<span data-ttu-id="c9b48-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c9b48-114">Application</span></span> | <span data-ttu-id="c9b48-115">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="c9b48-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="c9b48-116">除了权限范围，此 API 要求具有至少一个角色分配对资源的请求程序。</span><span class="sxs-lookup"><span data-stu-id="c9b48-116">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="c9b48-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c9b48-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions
GET /privilegedAccess/azureResources/roleDefinitions?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c9b48-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c9b48-118">Optional query parameters</span></span>
<span data-ttu-id="c9b48-119">此方法支持[OData 查询参数](/graph/query-parameters)以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="c9b48-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c9b48-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c9b48-120">Request headers</span></span>
| <span data-ttu-id="c9b48-121">名称</span><span class="sxs-lookup"><span data-stu-id="c9b48-121">Name</span></span>      |<span data-ttu-id="c9b48-122">说明</span><span class="sxs-lookup"><span data-stu-id="c9b48-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c9b48-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9b48-123">Authorization</span></span>  | <span data-ttu-id="c9b48-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c9b48-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9b48-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c9b48-125">Request body</span></span>
<span data-ttu-id="c9b48-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c9b48-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c9b48-127">响应</span><span class="sxs-lookup"><span data-stu-id="c9b48-127">Response</span></span>
<span data-ttu-id="c9b48-128">如果成功，此方法返回`200 OK`响应代码和响应正文中的[governanceRoleDefinition](../resources/governanceroledefinition.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="c9b48-128">If successful, this method returns a `200 OK` response code and collection of [governanceRoleDefinition](../resources/governanceroledefinition.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c9b48-129">示例</span><span class="sxs-lookup"><span data-stu-id="c9b48-129">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinitions"
}-->
<span data-ttu-id="c9b48-130">本示例演示如何获取 Wingtip Toys-prod 移的订阅的所有角色定义。</span><span class="sxs-lookup"><span data-stu-id="c9b48-130">This example shows how to get all role definitions of the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="c9b48-131">请求</span><span class="sxs-lookup"><span data-stu-id="c9b48-131">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions  
```
##### <a name="response"></a><span data-ttu-id="c9b48-132">响应</span><span class="sxs-lookup"><span data-stu-id="c9b48-132">Response</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroledefinition-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
