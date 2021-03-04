---
title: 列出 privilegedRoleAssignments
description: 检索 privilegedRoleAssignment 对象的列表，这些对象对应于组织的所有角色分配。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: a7dc26effcc7d43348e05f57dc54e1f908ea79c7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441226"
---
# <a name="list-privilegedroleassignments"></a><span data-ttu-id="13911-103">列出 privilegedRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="13911-103">List privilegedRoleAssignments</span></span>

<span data-ttu-id="13911-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13911-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13911-105">检索 [privilegedRoleAssignment](../resources/privilegedroleassignment.md) 对象的列表，这些对象对应于组织的所有角色分配。</span><span class="sxs-lookup"><span data-stu-id="13911-105">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects, which correspond to all role assignments for the organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="13911-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="13911-106">Permissions</span></span>
<span data-ttu-id="13911-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="13911-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="13911-109">请求者需要具有以下角色之一 _：Privileged Role Administrator、Global_ _Administrator、Security_ _Administrator_ 或 _Security Reader。_</span><span class="sxs-lookup"><span data-stu-id="13911-109">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="13911-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="13911-110">Permission type</span></span>      | <span data-ttu-id="13911-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="13911-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13911-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="13911-112">Delegated (work or school account)</span></span> | <span data-ttu-id="13911-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="13911-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="13911-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="13911-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13911-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="13911-115">Not supported.</span></span>    |
|<span data-ttu-id="13911-116">Application</span><span class="sxs-lookup"><span data-stu-id="13911-116">Application</span></span> | <span data-ttu-id="13911-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="13911-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="13911-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="13911-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="13911-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="13911-119">Optional query parameters</span></span>
<span data-ttu-id="13911-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="13911-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="13911-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="13911-121">Request headers</span></span>
| <span data-ttu-id="13911-122">名称</span><span class="sxs-lookup"><span data-stu-id="13911-122">Name</span></span>      |<span data-ttu-id="13911-123">说明</span><span class="sxs-lookup"><span data-stu-id="13911-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="13911-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="13911-124">Authorization</span></span>  | <span data-ttu-id="13911-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="13911-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13911-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="13911-127">Request body</span></span>
<span data-ttu-id="13911-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="13911-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13911-129">响应</span><span class="sxs-lookup"><span data-stu-id="13911-129">Response</span></span>

<span data-ttu-id="13911-130">如果成功，此方法在响应正文中返回 `200 OK` [响应代码和 privilegedRoleAssignment](../resources/privilegedroleassignment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="13911-130">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="13911-131">请注意，租户需要注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="13911-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="13911-132">否则，将返回 HTTP 403 禁止状态代码。</span><span class="sxs-lookup"><span data-stu-id="13911-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="examples"></a><span data-ttu-id="13911-133">示例</span><span class="sxs-lookup"><span data-stu-id="13911-133">Examples</span></span>
### <a name="get-all-role-assignments"></a><span data-ttu-id="13911-134">获取所有角色分配</span><span class="sxs-lookup"><span data-stu-id="13911-134">Get all role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="13911-135">请求</span><span class="sxs-lookup"><span data-stu-id="13911-135">Request</span></span>
<span data-ttu-id="13911-136">以下示例显示获取所有角色分配的请求：</span><span class="sxs-lookup"><span data-stu-id="13911-136">The following example shows a request to get all role assignments:</span></span>

# <a name="http"></a>[<span data-ttu-id="13911-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="13911-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments
```
# <a name="c"></a>[<span data-ttu-id="13911-138">C#</span><span class="sxs-lookup"><span data-stu-id="13911-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="13911-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13911-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="13911-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="13911-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="13911-141">Java</span><span class="sxs-lookup"><span data-stu-id="13911-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="13911-142">响应</span><span class="sxs-lookup"><span data-stu-id="13911-142">Response</span></span>
<span data-ttu-id="13911-143">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="13911-143">The following example shows the response.</span></span> <span data-ttu-id="13911-144">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="13911-144">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="13911-145">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="13911-145">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-active-role-assignments"></a><span data-ttu-id="13911-146">获取活动角色分配</span><span class="sxs-lookup"><span data-stu-id="13911-146">Get active role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="13911-147">请求</span><span class="sxs-lookup"><span data-stu-id="13911-147">Request</span></span> 
<span data-ttu-id="13911-148">以下示例显示查询活动角色分配的请求：</span><span class="sxs-lookup"><span data-stu-id="13911-148">The following example shows a request to query active role assignments:</span></span>

# <a name="http"></a>[<span data-ttu-id="13911-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="13911-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true
```
# <a name="c"></a>[<span data-ttu-id="13911-150">C#</span><span class="sxs-lookup"><span data-stu-id="13911-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="13911-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13911-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="13911-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="13911-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="13911-153">Java</span><span class="sxs-lookup"><span data-stu-id="13911-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="13911-154">响应</span><span class="sxs-lookup"><span data-stu-id="13911-154">Response</span></span>
<span data-ttu-id="13911-155">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="13911-155">The following example shows the response.</span></span> <span data-ttu-id="13911-156">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="13911-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="13911-157">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="13911-157">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-permanent-role-assignments"></a><span data-ttu-id="13911-158">获取永久角色分配</span><span class="sxs-lookup"><span data-stu-id="13911-158">Get permanent role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="13911-159">请求</span><span class="sxs-lookup"><span data-stu-id="13911-159">Request</span></span> 
<span data-ttu-id="13911-160">以下示例显示查询永久角色分配的请求，其中 ``expirationDateTime`` 值为 ``null`` ：</span><span class="sxs-lookup"><span data-stu-id="13911-160">The following example shows a request to query permanent role assignments, where ``expirationDateTime`` value is ``null``:</span></span>

# <a name="http"></a>[<span data-ttu-id="13911-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="13911-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20eq%20null
```
# <a name="c"></a>[<span data-ttu-id="13911-162">C#</span><span class="sxs-lookup"><span data-stu-id="13911-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="13911-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13911-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="13911-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="13911-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="13911-165">Java</span><span class="sxs-lookup"><span data-stu-id="13911-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="13911-166">响应</span><span class="sxs-lookup"><span data-stu-id="13911-166">Response</span></span>
<span data-ttu-id="13911-167">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="13911-167">The following example shows the response.</span></span> <span data-ttu-id="13911-168">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="13911-168">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="13911-169">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="13911-169">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-eligible-role-assignments"></a><span data-ttu-id="13911-170">获取符合条件的角色分配</span><span class="sxs-lookup"><span data-stu-id="13911-170">Get eligible role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="13911-171">请求</span><span class="sxs-lookup"><span data-stu-id="13911-171">Request</span></span> 
<span data-ttu-id="13911-172">以下示例显示查询符合条件的角色分配的请求，包括活动角色分配和非活动角色分配：</span><span class="sxs-lookup"><span data-stu-id="13911-172">The following example shows a request to query eligible role assignments, including the active and non-active ones:</span></span>

# <a name="http"></a>[<span data-ttu-id="13911-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="13911-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20ne%20null%20or%20isElevated%20eq%20false
```
# <a name="c"></a>[<span data-ttu-id="13911-174">C#</span><span class="sxs-lookup"><span data-stu-id="13911-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="13911-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13911-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="13911-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="13911-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="13911-177">Java</span><span class="sxs-lookup"><span data-stu-id="13911-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="13911-178">响应</span><span class="sxs-lookup"><span data-stu-id="13911-178">Response</span></span> 
<span data-ttu-id="13911-179">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="13911-179">The following example shows the response.</span></span> <span data-ttu-id="13911-180">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="13911-180">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="13911-181">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="13911-181">All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
