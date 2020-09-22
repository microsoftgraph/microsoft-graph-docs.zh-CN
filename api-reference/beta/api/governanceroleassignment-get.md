---
title: 获取 governanceRoleAssignment
description: 检索 governanceRoleAssignment 的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 77b188d37ebab092caba83cb0b4cc1cd639f6df4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991150"
---
# <a name="get-governanceroleassignment"></a><span data-ttu-id="9d225-103">获取 governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="9d225-103">Get governanceRoleAssignment</span></span>

<span data-ttu-id="9d225-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d225-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d225-105">检索 [governanceRoleAssignment](../resources/governanceroleassignment.md)的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9d225-105">Retrieve the properties and relationships of a [governanceRoleAssignment](../resources/governanceroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9d225-106">权限</span><span class="sxs-lookup"><span data-stu-id="9d225-106">Permissions</span></span>
<span data-ttu-id="9d225-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9d225-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d225-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9d225-109">Permission type</span></span>      | <span data-ttu-id="9d225-110">权限</span><span class="sxs-lookup"><span data-stu-id="9d225-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d225-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9d225-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9d225-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="9d225-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="9d225-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9d225-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d225-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d225-114">Not supported.</span></span>    |
|<span data-ttu-id="9d225-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9d225-115">Application</span></span> | <span data-ttu-id="9d225-116">PrivilegedAccess。 AzureResources</span><span class="sxs-lookup"><span data-stu-id="9d225-116">PrivilegedAccess.Read.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d225-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9d225-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
1. <span data-ttu-id="9d225-118">获取资源的[governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9d225-118">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on a resource</span></span>

    <span data-ttu-id="9d225-119">*注意：除了权限范围之外，要求请求者至少具有对资源的一个角色分配。*</span><span class="sxs-lookup"><span data-stu-id="9d225-119">*Note: Besides the permission scope, it requires the requestor to have at least one role assignment on the resource.*</span></span> 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments/{id}
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=resourceId+eq+'{resourceId}'
```
2. <span data-ttu-id="9d225-120">获取地雷的[governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9d225-120">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=subjectId+eq+'{myId}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9d225-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9d225-121">Optional query parameters</span></span>
<span data-ttu-id="9d225-122">此方法不 **支持除** 之外的 [OData 查询参数](/graph/query-parameters) `$filter` 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9d225-122">This method does **not** supports [OData Query Parameters](/graph/query-parameters) other than `$filter` to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9d225-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="9d225-123">Request headers</span></span>
| <span data-ttu-id="9d225-124">名称</span><span class="sxs-lookup"><span data-stu-id="9d225-124">Name</span></span>      |<span data-ttu-id="9d225-125">说明</span><span class="sxs-lookup"><span data-stu-id="9d225-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9d225-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d225-126">Authorization</span></span>  | <span data-ttu-id="9d225-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9d225-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d225-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="9d225-128">Request body</span></span>
<span data-ttu-id="9d225-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9d225-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9d225-130">响应</span><span class="sxs-lookup"><span data-stu-id="9d225-130">Response</span></span>
<span data-ttu-id="9d225-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [governanceRoleAssignment](../resources/governanceroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9d225-131">If successful, this method returns a `200 OK` response code and [governanceRoleAssignment](../resources/governanceroleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9d225-132">示例</span><span class="sxs-lookup"><span data-stu-id="9d225-132">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignment"
}-->
<span data-ttu-id="9d225-133">获取订阅 "Wingtip 玩具-生产" 的[governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9d225-133">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on subscription "Wingtip Toys - Prod"</span></span>
##### <a name="request"></a><span data-ttu-id="9d225-134">请求</span><span class="sxs-lookup"><span data-stu-id="9d225-134">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/0ba78f41-ee7a-4227-adb9-1499431b2164?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="9d225-135">响应</span><span class="sxs-lookup"><span data-stu-id="9d225-135">Response</span></span>
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


