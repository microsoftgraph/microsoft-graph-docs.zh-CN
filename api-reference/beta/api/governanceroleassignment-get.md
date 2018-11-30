---
title: 获取 governanceRoleAssignment
description: 检索的属性和 governanceRoleAssignment 的关系。
ms.openlocfilehash: fd35b9ba8083f49044115b914339e1069ccce896
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044569"
---
# <a name="get-governanceroleassignment"></a><span data-ttu-id="cee9d-103">获取 governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="cee9d-103">Get governanceRoleAssignment</span></span>

> <span data-ttu-id="cee9d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cee9d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cee9d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cee9d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cee9d-106">检索的属性和[governanceRoleAssignment](../resources/governanceroleassignment.md)的关系。</span><span class="sxs-lookup"><span data-stu-id="cee9d-106">Retrieve the properties and relationships of a [governanceRoleAssignment](../resources/governanceroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cee9d-107">权限</span><span class="sxs-lookup"><span data-stu-id="cee9d-107">Permissions</span></span>
<span data-ttu-id="cee9d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cee9d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cee9d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cee9d-110">Permission type</span></span>      | <span data-ttu-id="cee9d-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="cee9d-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cee9d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cee9d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cee9d-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="cee9d-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="cee9d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cee9d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cee9d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cee9d-115">Not supported.</span></span>    |
|<span data-ttu-id="cee9d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cee9d-116">Application</span></span> | <span data-ttu-id="cee9d-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="cee9d-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="cee9d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cee9d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
1. <span data-ttu-id="cee9d-119">获取对资源的[governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="cee9d-119">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on a resource</span></span>

    <span data-ttu-id="cee9d-120">*注意： 权限范围，除了需要具有至少一个角色分配对资源的请求程序。*</span><span class="sxs-lookup"><span data-stu-id="cee9d-120">*Note: Besides the permission scope, it requires the requestor to have at least one role assignment on the resource.*</span></span> 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments/{id}
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=resourceId+eq+'{resourceId}'
```
2. <span data-ttu-id="cee9d-121">获取我的[governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="cee9d-121">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=subjectId+eq+'{myId}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cee9d-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cee9d-122">Optional query parameters</span></span>
<span data-ttu-id="cee9d-123">此方法**不支持[OData 查询参数](/graph/query-parameters)以外的其他**`$filter`以帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cee9d-123">This method does **not** supports [OData Query Parameters](/graph/query-parameters) other than `$filter` to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cee9d-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="cee9d-124">Request headers</span></span>
| <span data-ttu-id="cee9d-125">名称</span><span class="sxs-lookup"><span data-stu-id="cee9d-125">Name</span></span>      |<span data-ttu-id="cee9d-126">说明</span><span class="sxs-lookup"><span data-stu-id="cee9d-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cee9d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="cee9d-127">Authorization</span></span>  | <span data-ttu-id="cee9d-128">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="cee9d-128">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="cee9d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="cee9d-129">Request body</span></span>
<span data-ttu-id="cee9d-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cee9d-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="cee9d-131">响应</span><span class="sxs-lookup"><span data-stu-id="cee9d-131">Response</span></span>
<span data-ttu-id="cee9d-132">如果成功，此方法返回`200 OK`响应正文中的响应代码和[governanceRoleAssignment](../resources/governanceroleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cee9d-132">If successful, this method returns a `200 OK` response code and [governanceRoleAssignment](../resources/governanceroleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cee9d-133">示例</span><span class="sxs-lookup"><span data-stu-id="cee9d-133">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignment"
}-->
<span data-ttu-id="cee9d-134">获取订阅"Wingtip Toys-prod 移" [governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="cee9d-134">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on subscription "Wingtip Toys - Prod"</span></span>
##### <a name="request"></a><span data-ttu-id="cee9d-135">请求</span><span class="sxs-lookup"><span data-stu-id="cee9d-135">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/0ba78f41-ee7a-4227-adb9-1499431b2164?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="cee9d-136">响应</span><span class="sxs-lookup"><span data-stu-id="cee9d-136">Response</span></span>
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
    "isPermanent": false,
    "startDateTime": "2018-01-22T23:47:19.687Z",
    "endDateTime": "2018-07-21T23:47:02.887Z",
    "memberType": "Direct",
    "assignmentState": "Eligible",
    "status": "Provisioned"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->