---
title: 获取 governanceRoleAssignmentRequest
description: '获取 governanceRoleAssignmentRequest。 '
localization_priority: Normal
ms.openlocfilehash: 6914dbe8c45bcc05bc684b08fb5fdf87405a045a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524133"
---
# <a name="get-governanceroleassignmentrequest"></a><span data-ttu-id="6fb53-103">获取 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="6fb53-103">Get governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fb53-104">获取[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="6fb53-104">Get a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="6fb53-105">权限</span><span class="sxs-lookup"><span data-stu-id="6fb53-105">Permissions</span></span>
<span data-ttu-id="6fb53-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6fb53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fb53-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6fb53-108">Permission type</span></span>      | <span data-ttu-id="6fb53-109">权限</span><span class="sxs-lookup"><span data-stu-id="6fb53-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6fb53-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6fb53-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6fb53-111">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="6fb53-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="6fb53-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6fb53-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fb53-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6fb53-113">Not supported.</span></span>    |
|<span data-ttu-id="6fb53-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6fb53-114">Application</span></span> | <span data-ttu-id="6fb53-115">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="6fb53-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="6fb53-116">除了权限范围，它需要请求程序</span><span class="sxs-lookup"><span data-stu-id="6fb53-116">Besides the permission scope, it requires the requestor</span></span> 
*   <span data-ttu-id="6fb53-117">若要对资源; 具有至少一个角色分配或</span><span class="sxs-lookup"><span data-stu-id="6fb53-117">to have at least one role assignment on the resource; or</span></span>
*   <span data-ttu-id="6fb53-118">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)的主题。</span><span class="sxs-lookup"><span data-stu-id="6fb53-118">is the subject of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="6fb53-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6fb53-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleAssignmentRequests/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6fb53-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6fb53-120">Optional query parameters</span></span>
<span data-ttu-id="6fb53-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6fb53-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6fb53-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="6fb53-122">Request headers</span></span>
| <span data-ttu-id="6fb53-123">名称</span><span class="sxs-lookup"><span data-stu-id="6fb53-123">Name</span></span>      |<span data-ttu-id="6fb53-124">说明</span><span class="sxs-lookup"><span data-stu-id="6fb53-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6fb53-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fb53-125">Authorization</span></span>  | <span data-ttu-id="6fb53-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="6fb53-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fb53-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6fb53-127">Request body</span></span>
<span data-ttu-id="6fb53-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6fb53-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6fb53-129">响应</span><span class="sxs-lookup"><span data-stu-id="6fb53-129">Response</span></span>
<span data-ttu-id="6fb53-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6fb53-130">If successful, this method returns a `200 OK` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fb53-131">示例</span><span class="sxs-lookup"><span data-stu-id="6fb53-131">Example</span></span>
<span data-ttu-id="6fb53-132">获取一个角色分配请求</span><span class="sxs-lookup"><span data-stu-id="6fb53-132">Get a role assignment request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequest"
}-->
##### <a name="request"></a><span data-ttu-id="6fb53-133">请求</span><span class="sxs-lookup"><span data-stu-id="6fb53-133">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/e68ff888-4af5-4ccb-8b74-39156090344b
```
##### <a name="response"></a><span data-ttu-id="6fb53-134">响应</span><span class="sxs-lookup"><span data-stu-id="6fb53-134">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"e68ff888-4af5-4ccb-8b74-39156090344b",
  "resourceId":"ec3a00f7-81dc-43b3-bbe7-650d3a5f7d46",
  "roleDefinitionId":"be0767b9-2c31-4b0d-b820-726228e7ff5c",
  "subjectId":"a4c5a837-b546-4ec5-a7df-e61547a46a4b",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminRemove",
  "assignmentState":"Eligible",
  "requestedDateTime":"2018-05-09T21:26:15.73-07:00",
  "reason":null,
  "status":{
    "status":"Closed",
    "subStatus":"Revoked",
    "statusDetails":[]
  },
  "schedule":null
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
