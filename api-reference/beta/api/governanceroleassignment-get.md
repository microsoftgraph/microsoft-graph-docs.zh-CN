---
title: 获取 governanceRoleAssignment
description: 检索 governanceRoleAssignment 的属性和关系。
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identitiy-platform
ms.openlocfilehash: 038189ac8bda4b51588532cbddc022e83db9ffbf
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639847"
---
# <a name="get-governanceroleassignment"></a><span data-ttu-id="b006f-103">获取 governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="b006f-103">Get governanceRoleAssignment</span></span>

<span data-ttu-id="b006f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b006f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b006f-105">检索[governanceRoleAssignment](../resources/governanceroleassignment.md)的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b006f-105">Retrieve the properties and relationships of a [governanceRoleAssignment](../resources/governanceroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b006f-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="b006f-106">Permissions</span></span>
<span data-ttu-id="b006f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b006f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b006f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b006f-109">Permission type</span></span>      | <span data-ttu-id="b006f-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="b006f-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b006f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b006f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b006f-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="b006f-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="b006f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b006f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b006f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b006f-114">Not supported.</span></span>    |
|<span data-ttu-id="b006f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b006f-115">Application</span></span> | <span data-ttu-id="b006f-116">PrivilegedAccess。 AzureResources</span><span class="sxs-lookup"><span data-stu-id="b006f-116">PrivilegedAccess.Read.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="b006f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b006f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
1. <span data-ttu-id="b006f-118">获取资源的[governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b006f-118">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on a resource</span></span>

    <span data-ttu-id="b006f-119">*注意：除了权限范围之外，要求请求者至少具有对资源的一个角色分配。*</span><span class="sxs-lookup"><span data-stu-id="b006f-119">*Note: Besides the permission scope, it requires the requestor to have at least one role assignment on the resource.*</span></span> 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments/{id}
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=resourceId+eq+'{resourceId}'
```
2. <span data-ttu-id="b006f-120">获取地雷的[governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b006f-120">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=subjectId+eq+'{myId}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b006f-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b006f-121">Optional query parameters</span></span>
<span data-ttu-id="b006f-122">此方法不**支持除**之外`$filter`的[OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b006f-122">This method does **not** supports [OData Query Parameters](/graph/query-parameters) other than `$filter` to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b006f-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="b006f-123">Request headers</span></span>
| <span data-ttu-id="b006f-124">名称</span><span class="sxs-lookup"><span data-stu-id="b006f-124">Name</span></span>      |<span data-ttu-id="b006f-125">说明</span><span class="sxs-lookup"><span data-stu-id="b006f-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b006f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b006f-126">Authorization</span></span>  | <span data-ttu-id="b006f-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b006f-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b006f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b006f-128">Request body</span></span>
<span data-ttu-id="b006f-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b006f-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b006f-130">响应</span><span class="sxs-lookup"><span data-stu-id="b006f-130">Response</span></span>
<span data-ttu-id="b006f-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[governanceRoleAssignment](../resources/governanceroleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b006f-131">If successful, this method returns a `200 OK` response code and [governanceRoleAssignment](../resources/governanceroleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b006f-132">示例</span><span class="sxs-lookup"><span data-stu-id="b006f-132">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignment"
}-->
<span data-ttu-id="b006f-133">获取订阅 "Wingtip 玩具-生产" 的[governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b006f-133">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on subscription "Wingtip Toys - Prod"</span></span>
##### <a name="request"></a><span data-ttu-id="b006f-134">请求</span><span class="sxs-lookup"><span data-stu-id="b006f-134">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/0ba78f41-ee7a-4227-adb9-1499431b2164?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="b006f-135">响应</span><span class="sxs-lookup"><span data-stu-id="b006f-135">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 182

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignments/$entity",
    "id": "0ba78f41-ee7a-4227-adb9-1499431b2164",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
    "subjectId": "74487eb5-1630-4fa8-9581-0bb076ea5de3",
    "linkedEligibleRoleAssignmentId": null,
    "externalId": null,
    "startDateTime": "2018-01-22T23:47:19.687Z",
    "endDateTime": "2018-07-21T23:47:02.887Z",
    "memberType": "Direct",
    "assignmentState": "Eligible",
    "status": "Provisioned"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
