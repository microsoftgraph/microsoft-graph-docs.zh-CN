---
title: 导出 governanceRoleAssignmentRequests
description: 以格式`application/octet-stream`检索 governanceRoleAssignmentRequests 的集合, 可以在浏览器中将其解析为 .csv 文件。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 227968ab265c117e5fa297d8fd8d8a988ddd0028
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954282"
---
# <a name="export-governanceroleassignmentrequests"></a><span data-ttu-id="b10fe-103">导出 governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="b10fe-103">Export governanceRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b10fe-104">以格式`application/octet-stream`检索[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)的集合, 可以在浏览器中将其解析为 .csv 文件。</span><span class="sxs-lookup"><span data-stu-id="b10fe-104">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) in the format `application/octet-stream`, which can be parsed as a .csv file in the browser.</span></span>

## <a name="permissions"></a><span data-ttu-id="b10fe-105">权限</span><span class="sxs-lookup"><span data-stu-id="b10fe-105">Permissions</span></span>
<span data-ttu-id="b10fe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b10fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b10fe-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b10fe-108">Permission type</span></span>      | <span data-ttu-id="b10fe-109">权限</span><span class="sxs-lookup"><span data-stu-id="b10fe-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b10fe-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b10fe-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b10fe-111">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="b10fe-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="b10fe-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b10fe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b10fe-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b10fe-113">Not supported.</span></span>    |
|<span data-ttu-id="b10fe-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b10fe-114">Application</span></span> | <span data-ttu-id="b10fe-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b10fe-115">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="b10fe-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b10fe-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="b10fe-117">导出资源的[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="b10fe-117">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource</span></span>
    
><span data-ttu-id="b10fe-118">**注意:** 除了权限范围之外, 此请求还要求请求者在资源上至少有一个角色分配。</span><span class="sxs-lookup"><span data-stu-id="b10fe-118">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

<span data-ttu-id="b10fe-119">导出地雷的[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="b10fe-119">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b10fe-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b10fe-120">Optional query parameters</span></span>
<span data-ttu-id="b10fe-121">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b10fe-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b10fe-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="b10fe-122">Request headers</span></span>
| <span data-ttu-id="b10fe-123">名称</span><span class="sxs-lookup"><span data-stu-id="b10fe-123">Name</span></span>      |<span data-ttu-id="b10fe-124">说明</span><span class="sxs-lookup"><span data-stu-id="b10fe-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b10fe-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b10fe-125">Authorization</span></span>  | <span data-ttu-id="b10fe-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b10fe-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b10fe-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b10fe-127">Request body</span></span>
<span data-ttu-id="b10fe-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b10fe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b10fe-129">响应</span><span class="sxs-lookup"><span data-stu-id="b10fe-129">Response</span></span>
<span data-ttu-id="b10fe-130">如果成功, 此方法将`200 OK`返回响应代码和类型`application/octet-stream`的内容。</span><span class="sxs-lookup"><span data-stu-id="b10fe-130">If successful, this method returns a `200 OK` response code and content of type `application/octet-stream`.</span></span>

## <a name="example"></a><span data-ttu-id="b10fe-131">示例</span><span class="sxs-lookup"><span data-stu-id="b10fe-131">Example</span></span>
<span data-ttu-id="b10fe-132">本示例将所有角色分配作为 .csv 文件保存在订阅 Wingtip 玩具-生产中。</span><span class="sxs-lookup"><span data-stu-id="b10fe-132">This example saves all role assignments as a .csv file in the subscription Wingtip Toys - Prod.</span></span> 

##### <a name="request"></a><span data-ttu-id="b10fe-133">请求</span><span class="sxs-lookup"><span data-stu-id="b10fe-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/export?filter=resourceId+eq+'85dfe48a-55d3-49fc-8f36-ee14b7f6f720'
```
##### <a name="response"></a><span data-ttu-id="b10fe-134">响应</span><span class="sxs-lookup"><span data-stu-id="b10fe-134">Response</span></span>
<span data-ttu-id="b10fe-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b10fe-135">Here is an example of the response.</span></span> 
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
  "suppressions": []
}
-->
