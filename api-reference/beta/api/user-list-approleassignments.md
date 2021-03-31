---
title: 列出向用户授予的 appRoleAssignment
description: 检索授予用户的应用角色分配的列表。
localization_priority: Priority
doc_type: apiPageType
ms.prod: users
author: psignoret
ms.openlocfilehash: 5e3e88a09408d44a07c34bf5379b189ada7055d9
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468693"
---
# <a name="list-approleassignments-granted-to-a-user"></a><span data-ttu-id="d9f09-103">列出向用户授予的 appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="d9f09-103">List appRoleAssignments granted to a user</span></span>

<span data-ttu-id="d9f09-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9f09-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9f09-105">检索授予用户的 [appRoleAssignment](../resources/approleassignment.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="d9f09-105">Retrieve the list of [appRoleAssignment](../resources/approleassignment.md) that a user has been granted.</span></span> <span data-ttu-id="d9f09-106">此操作也会返回分配给用户是其直接成员的组的应用角色。</span><span class="sxs-lookup"><span data-stu-id="d9f09-106">This operation also returns app roles assigned to groups that the user is a direct member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9f09-107">权限</span><span class="sxs-lookup"><span data-stu-id="d9f09-107">Permissions</span></span>

<span data-ttu-id="d9f09-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d9f09-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9f09-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d9f09-110">Permission type</span></span>      | <span data-ttu-id="d9f09-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d9f09-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9f09-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d9f09-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d9f09-113">Directory.Read.All、AppRoleAssignment.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d9f09-113">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="d9f09-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d9f09-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9f09-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9f09-115">Not supported.</span></span>    |
|<span data-ttu-id="d9f09-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d9f09-116">Application</span></span> | <span data-ttu-id="d9f09-117">Directory.Read.All、AppRoleAssignment.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9f09-117">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9f09-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d9f09-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/appRoleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d9f09-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d9f09-119">Optional query parameters</span></span>

<span data-ttu-id="d9f09-120">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d9f09-120">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d9f09-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d9f09-121">Request headers</span></span>

| <span data-ttu-id="d9f09-122">名称</span><span class="sxs-lookup"><span data-stu-id="d9f09-122">Name</span></span>           | <span data-ttu-id="d9f09-123">说明</span><span class="sxs-lookup"><span data-stu-id="d9f09-123">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="d9f09-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9f09-124">Authorization</span></span>  | <span data-ttu-id="d9f09-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d9f09-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d9f09-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d9f09-127">Request body</span></span>

<span data-ttu-id="d9f09-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d9f09-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9f09-129">响应</span><span class="sxs-lookup"><span data-stu-id="d9f09-129">Response</span></span>

<span data-ttu-id="d9f09-130">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [appRoleAssignment](../resources/approleassignment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d9f09-130">If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d9f09-131">示例</span><span class="sxs-lookup"><span data-stu-id="d9f09-131">Examples</span></span>

### <a name="example-1-list-approleassignments-granted-to-a-user"></a><span data-ttu-id="d9f09-132">示例 1：授予用户的 List appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="d9f09-132">Example 1: List appRoleAssignments granted to a user</span></span>

#### <a name="request"></a><span data-ttu-id="d9f09-133">请求</span><span class="sxs-lookup"><span data-stu-id="d9f09-133">Request</span></span>

<span data-ttu-id="d9f09-134">下面的示例展示了检索已分配给用户的应用角色的请求。</span><span class="sxs-lookup"><span data-stu-id="d9f09-134">Here is an example of the request to retrieve the app roles that have been assigned to a user.</span></span>


# <a name="http"></a>[<span data-ttu-id="d9f09-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9f09-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_approleassignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/cdb555e3-b33e-4fd5-a427-17fadacbdfa7/appRoleAssignments
```
# <a name="c"></a>[<span data-ttu-id="d9f09-136">C#</span><span class="sxs-lookup"><span data-stu-id="d9f09-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-approleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9f09-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9f09-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-approleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9f09-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9f09-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-approleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d9f09-139">Java</span><span class="sxs-lookup"><span data-stu-id="d9f09-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-approleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d9f09-140">响应</span><span class="sxs-lookup"><span data-stu-id="d9f09-140">Response</span></span>

<span data-ttu-id="d9f09-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d9f09-141">The following is an example of the response.</span></span> 

><span data-ttu-id="d9f09-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d9f09-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "41W1zT6z1U-kJxf62svfp1HFE8pMZhxDun-ThPczmJE",
      "deletedDateTime": null,
      "appRoleId": "00000000-0000-0000-0000-000000000000",
      "creationTimestamp": "2021-02-02T04:22:45.9480566Z",
      "principalDisplayName": "Alex Wilber",
      "principalId": "cdb555e3-b33e-4fd5-a427-17fadacbdfa7",
      "principalType": "User",
      "resourceDisplayName": "dxprovisioning-graphapi-client",
      "resourceId": "8e881353-1735-45af-af21-ee1344582a4d"
    }
  ]
}
```

### <a name="example-2-list-approleassignments-granted-to-a-user-filtered-by-resourceid"></a><span data-ttu-id="d9f09-144">示例 2：已按 resourceId 筛选的已授予用户的 List appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="d9f09-144">Example 2: List appRoleAssignments granted to a user, filtered by resourceId</span></span>

#### <a name="request"></a><span data-ttu-id="d9f09-145">请求</span><span class="sxs-lookup"><span data-stu-id="d9f09-145">Request</span></span>

<span data-ttu-id="d9f09-146">以下是请求检索已分配给用户的应用角色（按 `resourceId`GUID 类型）进行筛选的请求。</span><span class="sxs-lookup"><span data-stu-id="d9f09-146">Here is an example of the request to retrieve the app roles that have been assigned to a user, filtering by a `resourceId`, which is a GUID type.</span></span>


# <a name="http"></a>[<span data-ttu-id="d9f09-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9f09-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_approleassignments_filterby_resourceId"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/cdb555e3-b33e-4fd5-a427-17fadacbdfa7/appRoleAssignments?$filter=resourceId eq 8e881353-1735-45af-af21-ee1344582a4d
```
# <a name="c"></a>[<span data-ttu-id="d9f09-148">C#</span><span class="sxs-lookup"><span data-stu-id="d9f09-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-approleassignments-filterby-resourceid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9f09-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9f09-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-approleassignments-filterby-resourceid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9f09-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9f09-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-approleassignments-filterby-resourceid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d9f09-151">Java</span><span class="sxs-lookup"><span data-stu-id="d9f09-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-approleassignments-filterby-resourceid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d9f09-152">响应</span><span class="sxs-lookup"><span data-stu-id="d9f09-152">Response</span></span>

<span data-ttu-id="d9f09-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d9f09-153">The following is an example of the response.</span></span> 

><span data-ttu-id="d9f09-154">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d9f09-154">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#appRoleAssignments",
  "value": [
    {
      "id": "41W1zT6z1U-kJxf62svfp1HFE8pMZhxDun-ThPczmJE",
      "creationTimestamp": "2021-02-02T04:22:45.9480566Z",
      "appRoleId": "00000000-0000-0000-0000-000000000000",
      "principalDisplayName": "MOD Administrator",
      "principalId": "cdb555e3-b33e-4fd5-a427-17fadacbdfa7",
      "principalType": "User",
      "resourceDisplayName": "dxprovisioning-graphapi-client",
      "resourceId": "8e881353-1735-45af-af21-ee1344582a4d"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List appRoleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

