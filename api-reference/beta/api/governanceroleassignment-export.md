---
title: 导出 governanceRoleAssignmentRequests
description: 检索的格式 governanceRoleAssignmentRequests 集合`application/octet-stream`，其中可以解析为浏览器中的.csv 文件。
localization_priority: Normal
ms.openlocfilehash: 10fd7c720bf7b6f162a4d8c2189e81a9205e53ff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828726"
---
# <a name="export-governanceroleassignmentrequests"></a><span data-ttu-id="312c5-103">导出 governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="312c5-103">Export governanceRoleAssignmentRequests</span></span>

> <span data-ttu-id="312c5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="312c5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="312c5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="312c5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="312c5-106">检索的格式[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)集合`application/octet-stream`，其中可以解析为浏览器中的.csv 文件。</span><span class="sxs-lookup"><span data-stu-id="312c5-106">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) in the format `application/octet-stream`, which can be parsed as a .csv file in the browser.</span></span>

## <a name="permissions"></a><span data-ttu-id="312c5-107">权限</span><span class="sxs-lookup"><span data-stu-id="312c5-107">Permissions</span></span>
<span data-ttu-id="312c5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="312c5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="312c5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="312c5-110">Permission type</span></span>      | <span data-ttu-id="312c5-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="312c5-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="312c5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="312c5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="312c5-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="312c5-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="312c5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="312c5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="312c5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="312c5-115">Not supported.</span></span>    |
|<span data-ttu-id="312c5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="312c5-116">Application</span></span> | <span data-ttu-id="312c5-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="312c5-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |


## <a name="http-request"></a><span data-ttu-id="312c5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="312c5-118">HTTP request</span></span>
<span data-ttu-id="312c5-119"><!-- { "blockType": "ignored" } -->导出[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)对资源的集合</span><span class="sxs-lookup"><span data-stu-id="312c5-119"><!-- { "blockType": "ignored" } --> Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource</span></span>
    
><span data-ttu-id="312c5-120">**注意：** 除了权限范围，该请求需要具有至少一个角色分配对资源的请求程序。</span><span class="sxs-lookup"><span data-stu-id="312c5-120">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

<span data-ttu-id="312c5-121">导出的我的[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="312c5-121">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="312c5-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="312c5-122">Optional query parameters</span></span>
<span data-ttu-id="312c5-123">此方法支持[OData 查询参数](/graph/query-parameters)以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="312c5-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="312c5-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="312c5-124">Request headers</span></span>
| <span data-ttu-id="312c5-125">名称</span><span class="sxs-lookup"><span data-stu-id="312c5-125">Name</span></span>      |<span data-ttu-id="312c5-126">说明</span><span class="sxs-lookup"><span data-stu-id="312c5-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="312c5-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="312c5-127">Authorization</span></span>  | <span data-ttu-id="312c5-128">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="312c5-128">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="312c5-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="312c5-129">Request body</span></span>
<span data-ttu-id="312c5-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="312c5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="312c5-131">响应</span><span class="sxs-lookup"><span data-stu-id="312c5-131">Response</span></span>
<span data-ttu-id="312c5-132">如果成功，此方法返回`200 OK`响应代码和内容类型的`application/octet-stream`。</span><span class="sxs-lookup"><span data-stu-id="312c5-132">If successful, this method returns a `200 OK` response code and content of type `application/octet-stream`.</span></span>

## <a name="example"></a><span data-ttu-id="312c5-133">示例</span><span class="sxs-lookup"><span data-stu-id="312c5-133">Example</span></span>
<span data-ttu-id="312c5-134">本示例保存为.csv 文件订阅 Wingtip Toys-prod 移中的所有角色分配。</span><span class="sxs-lookup"><span data-stu-id="312c5-134">This example saves all role assignments as a .csv file in the subscription Wingtip Toys - Prod.</span></span> 

##### <a name="request"></a><span data-ttu-id="312c5-135">请求</span><span class="sxs-lookup"><span data-stu-id="312c5-135">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/export?filter=resourceId+eq+'85dfe48a-55d3-49fc-8f36-ee14b7f6f720'
```
##### <a name="response"></a><span data-ttu-id="312c5-136">响应</span><span class="sxs-lookup"><span data-stu-id="312c5-136">Response</span></span>
<span data-ttu-id="312c5-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="312c5-137">Here is an example of the response.</span></span> 
```http
HTTP/1.1 200 OK
Content-Type:application/octet-stream
Content-Length:126

77u/77u/QXNzaWdubWVudCBMZXZlbCxVc2VyIEdyb3VwIE5hbWUsUm9sZSBOYW1lLEVtYWlsLEFzc2lnbm1lbnQgVHlwZSxBc3NpZ25tZW43IFN0YXJ0IFRpbWUgKFVUQyksQXNzaWdubWVudCBFbmQgVGltZdAoVVRDKQ0K

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Export governanceRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
