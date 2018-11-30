---
title: 列表 governanceRoleAssignments
description: 检索 governanceRoleAssignments 的集合。
ms.openlocfilehash: 4b47756f75c7da1b0e9293eda449c5a244d015b6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041926"
---
# <a name="list-governanceroleassignments"></a><span data-ttu-id="a00c8-103">列表 governanceRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="a00c8-103">List governanceRoleAssignments</span></span>

> <span data-ttu-id="a00c8-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a00c8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a00c8-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a00c8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a00c8-106">检索[governanceRoleAssignments](../resources/governanceroleassignment.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="a00c8-106">Retrieve a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a00c8-107">权限</span><span class="sxs-lookup"><span data-stu-id="a00c8-107">Permissions</span></span>
<span data-ttu-id="a00c8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a00c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a00c8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a00c8-110">Permission type</span></span>      | <span data-ttu-id="a00c8-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="a00c8-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a00c8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a00c8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a00c8-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="a00c8-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="a00c8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a00c8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a00c8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a00c8-115">Not supported.</span></span>    |
|<span data-ttu-id="a00c8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a00c8-116">Application</span></span> | <span data-ttu-id="a00c8-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="a00c8-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |


## <a name="http-request"></a><span data-ttu-id="a00c8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a00c8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="a00c8-119">列出[governanceRoleAssignments](../resources/governanceroleassignment.md)对资源的集合。</span><span class="sxs-lookup"><span data-stu-id="a00c8-119">List a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md) on a resource.</span></span>

><span data-ttu-id="a00c8-120">**注意：** 除了权限范围，该请求需要具有至少一个角色分配对资源的请求程序。</span><span class="sxs-lookup"><span data-stu-id="a00c8-120">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments
GET /privilegedAccess/azureResources/roleAssignments?$filter=resourceId+eq+'{resourceId}'
```
<span data-ttu-id="a00c8-121">列出的[governanceRoleAssignments](../resources/governanceroleassignment.md)我的集合。</span><span class="sxs-lookup"><span data-stu-id="a00c8-121">List a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md) of mine.</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a00c8-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a00c8-122">Optional query parameters</span></span>
<span data-ttu-id="a00c8-123">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a00c8-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a00c8-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="a00c8-124">Request headers</span></span>
| <span data-ttu-id="a00c8-125">名称</span><span class="sxs-lookup"><span data-stu-id="a00c8-125">Name</span></span>      |<span data-ttu-id="a00c8-126">说明</span><span class="sxs-lookup"><span data-stu-id="a00c8-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a00c8-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="a00c8-127">Authorization</span></span>  | <span data-ttu-id="a00c8-128">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a00c8-128">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="a00c8-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a00c8-129">Request body</span></span>
<span data-ttu-id="a00c8-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a00c8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a00c8-131">响应</span><span class="sxs-lookup"><span data-stu-id="a00c8-131">Response</span></span>
<span data-ttu-id="a00c8-132">如果成功，此方法返回`200 OK`响应代码和响应正文中的[governanceRoleAssignment](../resources/governanceroleassignment.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="a00c8-132">If successful, this method returns a `200 OK` response code and a collection of [governanceRoleAssignment](../resources/governanceroleassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a00c8-133">示例</span><span class="sxs-lookup"><span data-stu-id="a00c8-133">Example</span></span>

<span data-ttu-id="a00c8-134">本示例演示如何获取我角色分配的订阅 Wingtip Toys-prod 移。</span><span class="sxs-lookup"><span data-stu-id="a00c8-134">This example shows how to get my role assignments on the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignments"
}-->
##### <a name="request"></a><span data-ttu-id="a00c8-135">请求</span><span class="sxs-lookup"><span data-stu-id="a00c8-135">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments?$filter=subjectId+eq+'918e54be-12c4-4f4c-a6d3-2ee0e3661c51'
```
##### <a name="response"></a><span data-ttu-id="a00c8-136">响应</span><span class="sxs-lookup"><span data-stu-id="a00c8-136">Response</span></span>
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
            "isPermanent": false,
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
            "isPermanent": false,
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
<!-- {
  "type": "#page.annotation",
  "description": "List roleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
