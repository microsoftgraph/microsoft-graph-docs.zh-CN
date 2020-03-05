---
title: 列出 governanceRoleAssignments
description: 检索 governanceRoleAssignments 的集合。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 0ab0b9b7d94891827489283b67d57c306770f057
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42421163"
---
# <a name="list-governanceroleassignments"></a><span data-ttu-id="4a7e5-103">列出 governanceRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="4a7e5-103">List governanceRoleAssignments</span></span>

<span data-ttu-id="4a7e5-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4a7e5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a7e5-105">检索[governanceRoleAssignments](../resources/governanceroleassignment.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="4a7e5-105">Retrieve a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4a7e5-106">权限</span><span class="sxs-lookup"><span data-stu-id="4a7e5-106">Permissions</span></span>
<span data-ttu-id="4a7e5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4a7e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a7e5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4a7e5-109">Permission type</span></span>      | <span data-ttu-id="4a7e5-110">权限</span><span class="sxs-lookup"><span data-stu-id="4a7e5-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a7e5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4a7e5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4a7e5-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="4a7e5-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="4a7e5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4a7e5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a7e5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4a7e5-114">Not supported.</span></span>    |
|<span data-ttu-id="4a7e5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4a7e5-115">Application</span></span> | <span data-ttu-id="4a7e5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4a7e5-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="4a7e5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4a7e5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="4a7e5-118">列出资源上的[governanceRoleAssignments](../resources/governanceroleassignment.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="4a7e5-118">List a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md) on a resource.</span></span>

><span data-ttu-id="4a7e5-119">**注意：** 除了权限范围之外，此请求还要求请求者在资源上至少有一个角色分配。</span><span class="sxs-lookup"><span data-stu-id="4a7e5-119">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments
GET /privilegedAccess/azureResources/roleAssignments?$filter=resourceId+eq+'{resourceId}'
```
<span data-ttu-id="4a7e5-120">列出地雷的[governanceRoleAssignments](../resources/governanceroleassignment.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="4a7e5-120">List a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md) of mine.</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4a7e5-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4a7e5-121">Optional query parameters</span></span>
<span data-ttu-id="4a7e5-122">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4a7e5-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a7e5-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="4a7e5-123">Request headers</span></span>
| <span data-ttu-id="4a7e5-124">名称</span><span class="sxs-lookup"><span data-stu-id="4a7e5-124">Name</span></span>      |<span data-ttu-id="4a7e5-125">说明</span><span class="sxs-lookup"><span data-stu-id="4a7e5-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4a7e5-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a7e5-126">Authorization</span></span>  | <span data-ttu-id="4a7e5-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="4a7e5-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a7e5-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="4a7e5-128">Request body</span></span>
<span data-ttu-id="4a7e5-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4a7e5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a7e5-130">响应</span><span class="sxs-lookup"><span data-stu-id="4a7e5-130">Response</span></span>
<span data-ttu-id="4a7e5-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[governanceRoleAssignment](../resources/governanceroleassignment.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="4a7e5-131">If successful, this method returns a `200 OK` response code and a collection of [governanceRoleAssignment](../resources/governanceroleassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4a7e5-132">示例</span><span class="sxs-lookup"><span data-stu-id="4a7e5-132">Example</span></span>

<span data-ttu-id="4a7e5-133">本示例演示如何在订阅 Wingtip 玩具-生产中获取我的角色分配。</span><span class="sxs-lookup"><span data-stu-id="4a7e5-133">This example shows how to get my role assignments on the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignments"
}-->
##### <a name="request"></a><span data-ttu-id="4a7e5-134">请求</span><span class="sxs-lookup"><span data-stu-id="4a7e5-134">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments?$filter=subjectId+eq+'918e54be-12c4-4f4c-a6d3-2ee0e3661c51'
```
##### <a name="response"></a><span data-ttu-id="4a7e5-135">响应</span><span class="sxs-lookup"><span data-stu-id="4a7e5-135">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 2062

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignments",
    "value": [
        {
            "id": "20f4157d-5837-4356-9630-ebd3a832f227",
            "resourceId": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
            "roleDefinitionId": "bc75b4e6-7403-4243-bf2f-d1f6990be122",
            "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
            "linkedEligibleRoleAssignmentId": null,
            "externalId": null,
            "startDateTime": "2018-03-13T01:19:08.59Z",
            "endDateTime": "2018-06-11T01:18:37.08Z",
            "memberType": "Direct",
            "assignmentState": "Eligible",
            "status": "Provisioned"
        },
        {
            "id": "e327f4be-42a0-47a2-8579-0a39b025b394",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
            "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
            "linkedEligibleRoleAssignmentId": null,
            "externalId": null,
            "startDateTime": "2018-03-28T16:56:48.243Z",
            "endDateTime": "2018-09-24T16:56:30.547Z",
            "memberType": "Direct",
            "assignmentState": "Eligible",
            "status": "Provisioned"
        },
        ...
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List roleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
