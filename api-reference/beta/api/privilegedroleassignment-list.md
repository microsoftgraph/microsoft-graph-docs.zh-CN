---
title: 列出 privilegedRoleAssignments
description: 检索 privilegedRoleAssignment 对象的列表，这些对象对应于组织的所有角色分配。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 01ca1661045d2f6c5695ad3879beec3cf9f5bf5e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049861"
---
# <a name="list-privilegedroleassignments"></a><span data-ttu-id="220ac-103">列出 privilegedRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="220ac-103">List privilegedRoleAssignments</span></span>

<span data-ttu-id="220ac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="220ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="220ac-105">检索 [privilegedRoleAssignment](../resources/privilegedroleassignment.md) 对象的列表，这些对象对应于组织的所有角色分配。</span><span class="sxs-lookup"><span data-stu-id="220ac-105">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects, which correspond to all role assignments for the organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="220ac-106">权限</span><span class="sxs-lookup"><span data-stu-id="220ac-106">Permissions</span></span>
<span data-ttu-id="220ac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="220ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="220ac-109">请求程序需要具有以下角色之一 _：Privileged Role Administrator、Global_ _Administrator、Security_ _Administrator_ 或 _Security Reader。_</span><span class="sxs-lookup"><span data-stu-id="220ac-109">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="220ac-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="220ac-110">Permission type</span></span>      | <span data-ttu-id="220ac-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="220ac-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="220ac-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="220ac-112">Delegated (work or school account)</span></span> | <span data-ttu-id="220ac-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="220ac-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="220ac-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="220ac-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="220ac-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="220ac-115">Not supported.</span></span>    |
|<span data-ttu-id="220ac-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="220ac-116">Application</span></span> | <span data-ttu-id="220ac-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="220ac-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="220ac-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="220ac-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="220ac-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="220ac-119">Optional query parameters</span></span>
<span data-ttu-id="220ac-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="220ac-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="220ac-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="220ac-121">Request headers</span></span>
| <span data-ttu-id="220ac-122">名称</span><span class="sxs-lookup"><span data-stu-id="220ac-122">Name</span></span>      |<span data-ttu-id="220ac-123">说明</span><span class="sxs-lookup"><span data-stu-id="220ac-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="220ac-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="220ac-124">Authorization</span></span>  | <span data-ttu-id="220ac-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="220ac-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="220ac-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="220ac-127">Request body</span></span>
<span data-ttu-id="220ac-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="220ac-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="220ac-129">响应</span><span class="sxs-lookup"><span data-stu-id="220ac-129">Response</span></span>

<span data-ttu-id="220ac-130">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [privilegedRoleAssignment](../resources/privilegedroleassignment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="220ac-130">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="220ac-131">请注意，租户需要注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="220ac-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="220ac-132">否则，将返回 HTTP 403 禁止状态代码。</span><span class="sxs-lookup"><span data-stu-id="220ac-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="examples"></a><span data-ttu-id="220ac-133">示例</span><span class="sxs-lookup"><span data-stu-id="220ac-133">Examples</span></span>
### <a name="get-all-role-assignments"></a><span data-ttu-id="220ac-134">获取所有角色分配</span><span class="sxs-lookup"><span data-stu-id="220ac-134">Get all role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="220ac-135">请求</span><span class="sxs-lookup"><span data-stu-id="220ac-135">Request</span></span>
<span data-ttu-id="220ac-136">以下示例显示获取所有角色分配的请求：</span><span class="sxs-lookup"><span data-stu-id="220ac-136">The following example shows a request to get all role assignments:</span></span>

# <a name="http"></a>[<span data-ttu-id="220ac-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="220ac-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments
```
# <a name="c"></a>[<span data-ttu-id="220ac-138">C#</span><span class="sxs-lookup"><span data-stu-id="220ac-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="220ac-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="220ac-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="220ac-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="220ac-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="220ac-141">Java</span><span class="sxs-lookup"><span data-stu-id="220ac-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignments-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="220ac-142">响应</span><span class="sxs-lookup"><span data-stu-id="220ac-142">Response</span></span>
<span data-ttu-id="220ac-143">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="220ac-143">The following example shows the response.</span></span> <span data-ttu-id="220ac-144">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="220ac-144">Note: The response object shown here might be shortened for readability.</span></span>
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
### <a name="get-active-role-assignments"></a><span data-ttu-id="220ac-145">获取活动角色分配</span><span class="sxs-lookup"><span data-stu-id="220ac-145">Get active role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="220ac-146">请求</span><span class="sxs-lookup"><span data-stu-id="220ac-146">Request</span></span> 
<span data-ttu-id="220ac-147">以下示例显示查询活动角色分配的请求：</span><span class="sxs-lookup"><span data-stu-id="220ac-147">The following example shows a request to query active role assignments:</span></span>

# <a name="http"></a>[<span data-ttu-id="220ac-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="220ac-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true
```
# <a name="c"></a>[<span data-ttu-id="220ac-149">C#</span><span class="sxs-lookup"><span data-stu-id="220ac-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="220ac-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="220ac-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="220ac-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="220ac-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="220ac-152">Java</span><span class="sxs-lookup"><span data-stu-id="220ac-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignments-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="220ac-153">响应</span><span class="sxs-lookup"><span data-stu-id="220ac-153">Response</span></span>
<span data-ttu-id="220ac-154">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="220ac-154">The following example shows the response.</span></span> <span data-ttu-id="220ac-155">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="220ac-155">Note: The response object shown here might be shortened for readability.</span></span>
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
### <a name="get-permanent-role-assignments"></a><span data-ttu-id="220ac-156">获取永久角色分配</span><span class="sxs-lookup"><span data-stu-id="220ac-156">Get permanent role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="220ac-157">请求</span><span class="sxs-lookup"><span data-stu-id="220ac-157">Request</span></span> 
<span data-ttu-id="220ac-158">以下示例显示查询永久角色分配的请求，其中 ``expirationDateTime`` value 为 ``null`` ：</span><span class="sxs-lookup"><span data-stu-id="220ac-158">The following example shows a request to query permanent role assignments, where ``expirationDateTime`` value is ``null``:</span></span>

# <a name="http"></a>[<span data-ttu-id="220ac-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="220ac-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20eq%20null
```
# <a name="c"></a>[<span data-ttu-id="220ac-160">C#</span><span class="sxs-lookup"><span data-stu-id="220ac-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="220ac-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="220ac-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="220ac-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="220ac-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="220ac-163">Java</span><span class="sxs-lookup"><span data-stu-id="220ac-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignments-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="220ac-164">响应</span><span class="sxs-lookup"><span data-stu-id="220ac-164">Response</span></span>
<span data-ttu-id="220ac-165">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="220ac-165">The following example shows the response.</span></span> <span data-ttu-id="220ac-166">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="220ac-166">Note: The response object shown here might be shortened for readability.</span></span>
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
### <a name="get-eligible-role-assignments"></a><span data-ttu-id="220ac-167">获取符合条件的角色分配</span><span class="sxs-lookup"><span data-stu-id="220ac-167">Get eligible role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="220ac-168">请求</span><span class="sxs-lookup"><span data-stu-id="220ac-168">Request</span></span> 
<span data-ttu-id="220ac-169">以下示例显示查询符合条件的角色分配的请求，包括活动和非活动角色分配：</span><span class="sxs-lookup"><span data-stu-id="220ac-169">The following example shows a request to query eligible role assignments, including the active and non-active ones:</span></span>

# <a name="http"></a>[<span data-ttu-id="220ac-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="220ac-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments_4"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20ne%20null%20or%20isElevated%20eq%20false
```
# <a name="c"></a>[<span data-ttu-id="220ac-171">C#</span><span class="sxs-lookup"><span data-stu-id="220ac-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="220ac-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="220ac-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="220ac-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="220ac-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="220ac-174">Java</span><span class="sxs-lookup"><span data-stu-id="220ac-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignments-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="220ac-175">响应</span><span class="sxs-lookup"><span data-stu-id="220ac-175">Response</span></span> 
<span data-ttu-id="220ac-176">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="220ac-176">The following example shows the response.</span></span> <span data-ttu-id="220ac-177">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="220ac-177">Note: The response object shown here might be shortened for readability.</span></span>
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
