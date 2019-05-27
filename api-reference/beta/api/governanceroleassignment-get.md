---
title: 获取 governanceRoleAssignment
description: 检索 governanceRoleAssignment 的属性和关系。
localization_priority: Normal
ms.openlocfilehash: e2e116baad573c8b99ab278771d1149ea3563209
ms.sourcegitcommit: f80282ff00d5aafc3e575bce447543d7dd23963d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/23/2019
ms.locfileid: "34422421"
---
# <a name="get-governanceroleassignment"></a><span data-ttu-id="2eec6-103">获取 governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="2eec6-103">Get governanceRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2eec6-104">检索[governanceRoleAssignment](../resources/governanceroleassignment.md)的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2eec6-104">Retrieve the properties and relationships of a [governanceRoleAssignment](../resources/governanceroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2eec6-105">权限</span><span class="sxs-lookup"><span data-stu-id="2eec6-105">Permissions</span></span>
<span data-ttu-id="2eec6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2eec6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2eec6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2eec6-108">Permission type</span></span>      | <span data-ttu-id="2eec6-109">权限</span><span class="sxs-lookup"><span data-stu-id="2eec6-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2eec6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2eec6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2eec6-111">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="2eec6-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="2eec6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2eec6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2eec6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2eec6-113">Not supported.</span></span>    |
|<span data-ttu-id="2eec6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2eec6-114">Application</span></span> | <span data-ttu-id="2eec6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2eec6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2eec6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2eec6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
1. <span data-ttu-id="2eec6-117">获取资源的[governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="2eec6-117">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on a resource</span></span>

    <span data-ttu-id="2eec6-118">*注意: 除了权限范围之外, 要求请求者至少具有对资源的一个角色分配。*</span><span class="sxs-lookup"><span data-stu-id="2eec6-118">*Note: Besides the permission scope, it requires the requestor to have at least one role assignment on the resource.*</span></span> 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments/{id}
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=resourceId+eq+'{resourceId}'
```
2. <span data-ttu-id="2eec6-119">获取地雷的[governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="2eec6-119">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=subjectId+eq+'{myId}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2eec6-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2eec6-120">Optional query parameters</span></span>
<span data-ttu-id="2eec6-121">此方法不\*\*\*\* 支持除之外`$filter`的[OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2eec6-121">This method does **not** supports [OData Query Parameters](/graph/query-parameters) other than `$filter` to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2eec6-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="2eec6-122">Request headers</span></span>
| <span data-ttu-id="2eec6-123">名称</span><span class="sxs-lookup"><span data-stu-id="2eec6-123">Name</span></span>      |<span data-ttu-id="2eec6-124">说明</span><span class="sxs-lookup"><span data-stu-id="2eec6-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2eec6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2eec6-125">Authorization</span></span>  | <span data-ttu-id="2eec6-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2eec6-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="2eec6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2eec6-127">Request body</span></span>
<span data-ttu-id="2eec6-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2eec6-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2eec6-129">响应</span><span class="sxs-lookup"><span data-stu-id="2eec6-129">Response</span></span>
<span data-ttu-id="2eec6-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[governanceRoleAssignment](../resources/governanceroleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2eec6-130">If successful, this method returns a `200 OK` response code and [governanceRoleAssignment](../resources/governanceroleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2eec6-131">示例</span><span class="sxs-lookup"><span data-stu-id="2eec6-131">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignment"
}-->
<span data-ttu-id="2eec6-132">获取订阅 "Wingtip 玩具-生产" 的[governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="2eec6-132">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on subscription "Wingtip Toys - Prod"</span></span>
##### <a name="request"></a><span data-ttu-id="2eec6-133">请求</span><span class="sxs-lookup"><span data-stu-id="2eec6-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/0ba78f41-ee7a-4227-adb9-1499431b2164?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="2eec6-134">响应</span><span class="sxs-lookup"><span data-stu-id="2eec6-134">Response</span></span>
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
