---
title: 导出 governanceRoleAssignmentRequests
description: 以格式`application/octet-stream`检索 governanceRoleAssignmentRequests 的集合，可以在浏览器中将其解析为 .csv 文件。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 616a6a7132d900fc57c2243bf86a372a23d37e77
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42421289"
---
# <a name="export-governanceroleassignmentrequests"></a><span data-ttu-id="a6bac-103">导出 governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="a6bac-103">Export governanceRoleAssignmentRequests</span></span>

<span data-ttu-id="a6bac-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a6bac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6bac-105">以格式`application/octet-stream`检索[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)的集合，可以在浏览器中将其解析为 .csv 文件。</span><span class="sxs-lookup"><span data-stu-id="a6bac-105">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) in the format `application/octet-stream`, which can be parsed as a .csv file in the browser.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6bac-106">权限</span><span class="sxs-lookup"><span data-stu-id="a6bac-106">Permissions</span></span>
<span data-ttu-id="a6bac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a6bac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6bac-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a6bac-109">Permission type</span></span>      | <span data-ttu-id="a6bac-110">权限</span><span class="sxs-lookup"><span data-stu-id="a6bac-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6bac-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a6bac-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a6bac-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="a6bac-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="a6bac-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a6bac-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6bac-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6bac-114">Not supported.</span></span>    |
|<span data-ttu-id="a6bac-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a6bac-115">Application</span></span> | <span data-ttu-id="a6bac-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6bac-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="a6bac-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a6bac-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="a6bac-118">导出资源的[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="a6bac-118">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource</span></span>
    
><span data-ttu-id="a6bac-119">**注意：** 除了权限范围之外，此请求还要求请求者在资源上至少有一个角色分配。</span><span class="sxs-lookup"><span data-stu-id="a6bac-119">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

<span data-ttu-id="a6bac-120">导出地雷的[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="a6bac-120">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a6bac-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a6bac-121">Optional query parameters</span></span>
<span data-ttu-id="a6bac-122">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a6bac-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a6bac-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="a6bac-123">Request headers</span></span>
| <span data-ttu-id="a6bac-124">名称</span><span class="sxs-lookup"><span data-stu-id="a6bac-124">Name</span></span>      |<span data-ttu-id="a6bac-125">说明</span><span class="sxs-lookup"><span data-stu-id="a6bac-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a6bac-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6bac-126">Authorization</span></span>  | <span data-ttu-id="a6bac-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a6bac-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6bac-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a6bac-128">Request body</span></span>
<span data-ttu-id="a6bac-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a6bac-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6bac-130">响应</span><span class="sxs-lookup"><span data-stu-id="a6bac-130">Response</span></span>
<span data-ttu-id="a6bac-131">如果成功，此方法将`200 OK`返回响应代码和类型`application/octet-stream`的内容。</span><span class="sxs-lookup"><span data-stu-id="a6bac-131">If successful, this method returns a `200 OK` response code and content of type `application/octet-stream`.</span></span>

## <a name="example"></a><span data-ttu-id="a6bac-132">示例</span><span class="sxs-lookup"><span data-stu-id="a6bac-132">Example</span></span>
<span data-ttu-id="a6bac-133">本示例将所有角色分配作为 .csv 文件保存在订阅 Wingtip 玩具-生产中。</span><span class="sxs-lookup"><span data-stu-id="a6bac-133">This example saves all role assignments as a .csv file in the subscription Wingtip Toys - Prod.</span></span> 

##### <a name="request"></a><span data-ttu-id="a6bac-134">请求</span><span class="sxs-lookup"><span data-stu-id="a6bac-134">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/export?filter=resourceId+eq+'85dfe48a-55d3-49fc-8f36-ee14b7f6f720'
```
##### <a name="response"></a><span data-ttu-id="a6bac-135">响应</span><span class="sxs-lookup"><span data-stu-id="a6bac-135">Response</span></span>
<span data-ttu-id="a6bac-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a6bac-136">Here is an example of the response.</span></span> 
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
