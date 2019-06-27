---
title: 列出 privilegedRoleAssignments
description: 检索 privilegedRoleAssignment 对象的列表, 这些对象对应于组织的所有角色分配。
localization_priority: Normal
ms.openlocfilehash: 6476f0c2a613de51914455fbd81089c995e44554
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268108"
---
# <a name="list-privilegedroleassignments"></a><span data-ttu-id="f8598-103">列出 privilegedRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="f8598-103">List privilegedRoleAssignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8598-104">检索[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象的列表, 这些对象对应于组织的所有角色分配。</span><span class="sxs-lookup"><span data-stu-id="f8598-104">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects, which correspond to all role assignments for the organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="f8598-105">权限</span><span class="sxs-lookup"><span data-stu-id="f8598-105">Permissions</span></span>
<span data-ttu-id="f8598-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f8598-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f8598-108">请求者需要具有以下角色之一:_特权角色管理员_、_全局管理员_、_安全管理员_或_安全读者_。</span><span class="sxs-lookup"><span data-stu-id="f8598-108">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="f8598-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8598-109">Permission type</span></span>      | <span data-ttu-id="f8598-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f8598-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8598-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8598-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f8598-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f8598-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f8598-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8598-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8598-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8598-114">Not supported.</span></span>    |
|<span data-ttu-id="f8598-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f8598-115">Application</span></span> | <span data-ttu-id="f8598-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8598-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8598-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8598-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f8598-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f8598-118">Optional query parameters</span></span>
<span data-ttu-id="f8598-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f8598-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f8598-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8598-120">Request headers</span></span>
| <span data-ttu-id="f8598-121">名称</span><span class="sxs-lookup"><span data-stu-id="f8598-121">Name</span></span>      |<span data-ttu-id="f8598-122">说明</span><span class="sxs-lookup"><span data-stu-id="f8598-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f8598-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8598-123">Authorization</span></span>  | <span data-ttu-id="f8598-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f8598-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8598-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f8598-126">Request body</span></span>
<span data-ttu-id="f8598-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f8598-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8598-128">响应</span><span class="sxs-lookup"><span data-stu-id="f8598-128">Response</span></span>

<span data-ttu-id="f8598-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="f8598-129">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="f8598-130">请注意, 需要将租户注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="f8598-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="f8598-131">否则, 将返回 HTTP 403 禁止的状态代码。</span><span class="sxs-lookup"><span data-stu-id="f8598-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="examples"></a><span data-ttu-id="f8598-132">示例</span><span class="sxs-lookup"><span data-stu-id="f8598-132">Examples</span></span>
### <a name="get-all-role-assignments"></a><span data-ttu-id="f8598-133">获取所有角色分配</span><span class="sxs-lookup"><span data-stu-id="f8598-133">Get all role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="f8598-134">请求</span><span class="sxs-lookup"><span data-stu-id="f8598-134">Request</span></span>
<span data-ttu-id="f8598-135">下面的示例展示了获取所有角色分配的请求:</span><span class="sxs-lookup"><span data-stu-id="f8598-135">The following example shows a request to get all role assignments:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments
```
##### <a name="response"></a><span data-ttu-id="f8598-136">响应</span><span class="sxs-lookup"><span data-stu-id="f8598-136">Response</span></span>
<span data-ttu-id="f8598-137">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="f8598-137">The following example shows the response.</span></span> <span data-ttu-id="f8598-138">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f8598-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f8598-139">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f8598-139">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "isElevated": true,
      "expirationDateTime": "2016-10-19T10:37:00Z",
      "resultMessage": "resultMessage-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f8598-140">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f8598-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f8598-141">C#</span><span class="sxs-lookup"><span data-stu-id="f8598-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_privilegedroleassignments-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f8598-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="f8598-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_privilegedroleassignments-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f8598-143">目标-C</span><span class="sxs-lookup"><span data-stu-id="f8598-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_privilegedroleassignments-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
### <a name="get-active-role-assignments"></a><span data-ttu-id="f8598-144">获取活动角色分配</span><span class="sxs-lookup"><span data-stu-id="f8598-144">Get active role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="f8598-145">请求</span><span class="sxs-lookup"><span data-stu-id="f8598-145">Request</span></span> 
<span data-ttu-id="f8598-146">以下示例显示查询活动角色分配的请求:</span><span class="sxs-lookup"><span data-stu-id="f8598-146">The following example shows a request to query active role assignments:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true
```
##### <a name="response"></a><span data-ttu-id="f8598-147">响应</span><span class="sxs-lookup"><span data-stu-id="f8598-147">Response</span></span>
<span data-ttu-id="f8598-148">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="f8598-148">The following example shows the response.</span></span> <span data-ttu-id="f8598-149">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f8598-149">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f8598-150">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f8598-150">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_62e90394-69f5-4237-9190-012177145e10",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "62e90394-69f5-4237-9190-012177145e10",
            "isElevated": true,
            "expirationDateTime": null,
            "resultMessage": null
        },
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "isElevated": true,
            "expirationDateTime": "2017-07-25T17:38:49.563Z",
            "resultMessage": null
        }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f8598-151">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f8598-151">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f8598-152">C#</span><span class="sxs-lookup"><span data-stu-id="f8598-152">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_privilegedroleassignments-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f8598-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="f8598-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_privilegedroleassignments-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f8598-154">目标-C</span><span class="sxs-lookup"><span data-stu-id="f8598-154">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_privilegedroleassignments-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
### <a name="get-permanent-role-assignments"></a><span data-ttu-id="f8598-155">获取永久角色分配</span><span class="sxs-lookup"><span data-stu-id="f8598-155">Get permanent role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="f8598-156">请求</span><span class="sxs-lookup"><span data-stu-id="f8598-156">Request</span></span> 
<span data-ttu-id="f8598-157">下面的示例演示了对查询永久角色分配的请求, ``expirationDateTime``其中 value ``null``是:</span><span class="sxs-lookup"><span data-stu-id="f8598-157">The following example shows a request to query permanent role assignments, where ``expirationDateTime`` value is ``null``:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20eq%20null
```
##### <a name="response"></a><span data-ttu-id="f8598-158">响应</span><span class="sxs-lookup"><span data-stu-id="f8598-158">Response</span></span>
<span data-ttu-id="f8598-159">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="f8598-159">The following example shows the response.</span></span> <span data-ttu-id="f8598-160">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f8598-160">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f8598-161">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f8598-161">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_194ae4cb-b126-40b2-bd5b-6091b380977d",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "194ae4cb-b126-40b2-bd5b-6091b380977d",
            "isElevated": true,
            "expirationDateTime": null,
            "resultMessage": null
        },
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_44367163-eba1-44c3-98af-f5787879f96a",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "44367163-eba1-44c3-98af-f5787879f96a",
            "isElevated": true,
            "expirationDateTime": null,
            "resultMessage": null
        }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f8598-162">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f8598-162">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f8598-163">C#</span><span class="sxs-lookup"><span data-stu-id="f8598-163">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_privilegedroleassignments-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f8598-164">Javascript</span><span class="sxs-lookup"><span data-stu-id="f8598-164">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_privilegedroleassignments-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f8598-165">目标-C</span><span class="sxs-lookup"><span data-stu-id="f8598-165">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_privilegedroleassignments-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
### <a name="get-eligible-role-assignments"></a><span data-ttu-id="f8598-166">获取符合条件的角色分配</span><span class="sxs-lookup"><span data-stu-id="f8598-166">Get eligible role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="f8598-167">请求</span><span class="sxs-lookup"><span data-stu-id="f8598-167">Request</span></span> 
<span data-ttu-id="f8598-168">以下示例显示查询符合条件的角色分配 (包括活动的和非活动的角色分配) 的请求:</span><span class="sxs-lookup"><span data-stu-id="f8598-168">The following example shows a request to query eligible role assignments, including the active and non-active ones:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20ne%20null%20or%20isElevated%20eq%20false
```
##### <a name="response"></a><span data-ttu-id="f8598-169">响应</span><span class="sxs-lookup"><span data-stu-id="f8598-169">Response</span></span> 
<span data-ttu-id="f8598-170">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="f8598-170">The following example shows the response.</span></span> <span data-ttu-id="f8598-171">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f8598-171">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f8598-172">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f8598-172">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "isElevated": true,
            "expirationDateTime": "2017-07-25T18:42:26.823Z",
            "resultMessage": null
        },
        {
            "id": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81_194ae4cb-b126-40b2-bd5b-6091b380977d",
            "userId": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81",
            "roleId": "194ae4cb-b126-40b2-bd5b-6091b380977d",
            "isElevated": false,
            "expirationDateTime": null,
            "resultMessage": null
        },
        {
            "id": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81_9360feb5-f418-4baa-8175-e2a00bac4301",
            "userId": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81",
            "roleId": "9360feb5-f418-4baa-8175-e2a00bac4301",
            "isElevated": false,
            "expirationDateTime": null,
            "resultMessage": null
        },
        {
            "id": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81_95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "userId": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "isElevated": false,
            "expirationDateTime": null,
            "resultMessage": null
        }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f8598-173">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f8598-173">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f8598-174">C#</span><span class="sxs-lookup"><span data-stu-id="f8598-174">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_privilegedroleassignments-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f8598-175">Javascript</span><span class="sxs-lookup"><span data-stu-id="f8598-175">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_privilegedroleassignments-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f8598-176">目标-C</span><span class="sxs-lookup"><span data-stu-id="f8598-176">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_privilegedroleassignments-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedRoleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignment-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/privilegedroleassignment-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedroleassignment-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/privilegedroleassignment-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedroleassignment-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/privilegedroleassignment-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedroleassignment-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/privilegedroleassignment-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedroleassignment-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
