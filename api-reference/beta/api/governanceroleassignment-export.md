---
title: 导出 governanceRoleAssignmentRequests
description: 检索的格式 governanceRoleAssignmentRequests 集合`application/octet-stream`，其中可以解析为浏览器中的.csv 文件。
localization_priority: Normal
ms.openlocfilehash: 82c36f176dfed1a4a848c045ce3274e1152bb953
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522425"
---
# <a name="export-governanceroleassignmentrequests"></a><span data-ttu-id="0eea9-103">导出 governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="0eea9-103">Export governanceRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0eea9-104">检索的格式[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)集合`application/octet-stream`，其中可以解析为浏览器中的.csv 文件。</span><span class="sxs-lookup"><span data-stu-id="0eea9-104">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) in the format `application/octet-stream`, which can be parsed as a .csv file in the browser.</span></span>

## <a name="permissions"></a><span data-ttu-id="0eea9-105">权限</span><span class="sxs-lookup"><span data-stu-id="0eea9-105">Permissions</span></span>
<span data-ttu-id="0eea9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0eea9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0eea9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0eea9-108">Permission type</span></span>      | <span data-ttu-id="0eea9-109">权限</span><span class="sxs-lookup"><span data-stu-id="0eea9-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0eea9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0eea9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0eea9-111">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="0eea9-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="0eea9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0eea9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0eea9-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0eea9-113">Not supported.</span></span>    |
|<span data-ttu-id="0eea9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0eea9-114">Application</span></span> | <span data-ttu-id="0eea9-115">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="0eea9-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |


## <a name="http-request"></a><span data-ttu-id="0eea9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0eea9-116">HTTP request</span></span>
<span data-ttu-id="0eea9-117"><!-- { "blockType": "ignored" } -->导出[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)对资源的集合</span><span class="sxs-lookup"><span data-stu-id="0eea9-117"><!-- { "blockType": "ignored" } --> Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource</span></span>
    
><span data-ttu-id="0eea9-118">**注意：** 除了权限范围，该请求需要具有至少一个角色分配对资源的请求程序。</span><span class="sxs-lookup"><span data-stu-id="0eea9-118">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

<span data-ttu-id="0eea9-119">导出的我的[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="0eea9-119">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0eea9-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0eea9-120">Optional query parameters</span></span>
<span data-ttu-id="0eea9-121">此方法支持[OData 查询参数](/graph/query-parameters)以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="0eea9-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0eea9-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="0eea9-122">Request headers</span></span>
| <span data-ttu-id="0eea9-123">名称</span><span class="sxs-lookup"><span data-stu-id="0eea9-123">Name</span></span>      |<span data-ttu-id="0eea9-124">说明</span><span class="sxs-lookup"><span data-stu-id="0eea9-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0eea9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0eea9-125">Authorization</span></span>  | <span data-ttu-id="0eea9-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0eea9-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="0eea9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0eea9-127">Request body</span></span>
<span data-ttu-id="0eea9-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0eea9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0eea9-129">响应</span><span class="sxs-lookup"><span data-stu-id="0eea9-129">Response</span></span>
<span data-ttu-id="0eea9-130">如果成功，此方法返回`200 OK`响应代码和内容类型的`application/octet-stream`。</span><span class="sxs-lookup"><span data-stu-id="0eea9-130">If successful, this method returns a `200 OK` response code and content of type `application/octet-stream`.</span></span>

## <a name="example"></a><span data-ttu-id="0eea9-131">示例</span><span class="sxs-lookup"><span data-stu-id="0eea9-131">Example</span></span>
<span data-ttu-id="0eea9-132">本示例保存为.csv 文件订阅 Wingtip Toys-prod 移中的所有角色分配。</span><span class="sxs-lookup"><span data-stu-id="0eea9-132">This example saves all role assignments as a .csv file in the subscription Wingtip Toys - Prod.</span></span> 

##### <a name="request"></a><span data-ttu-id="0eea9-133">请求</span><span class="sxs-lookup"><span data-stu-id="0eea9-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/export?filter=resourceId+eq+'85dfe48a-55d3-49fc-8f36-ee14b7f6f720'
```
##### <a name="response"></a><span data-ttu-id="0eea9-134">响应</span><span class="sxs-lookup"><span data-stu-id="0eea9-134">Response</span></span>
<span data-ttu-id="0eea9-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0eea9-135">Here is an example of the response.</span></span> 
```http
HTTP/1.1 200 OK
Content-Type:application/octet-stream
Content-Length:126

77u/77u/QXNzaWdubWVudCBMZXZlbCxVc2VyIEdyb3VwIE5hbWUsUm9sZSBOYW1lLEVtYWlsLEFzc2lnbm1lbnQgVHlwZSxBc3NpZ25tZW43IFN0YXJ0IFRpbWUgKFVUQyksQXNzaWdubWVudCBFbmQgVGltZdAoVVRDKQ0K

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Export governanceRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignment-export.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
