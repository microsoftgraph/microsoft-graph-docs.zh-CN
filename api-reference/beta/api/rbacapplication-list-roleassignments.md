---
title: 列出 unifiedRoleAssignments
description: 获取 unifiedRoleAssignment 对象的列表。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 08f23c997619c0d116bee75fed936145fea8ff71
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36725365"
---
# <a name="list-unifiedroleassignments"></a><span data-ttu-id="2d40b-103">列出 unifiedRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="2d40b-103">List unifiedRoleAssignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d40b-104">获取提供程序的[unifiedRoleAssignment](../resources/unifiedroleassignment.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="2d40b-104">Get a list of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) objects for the provider.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d40b-105">权限</span><span class="sxs-lookup"><span data-stu-id="2d40b-105">Permissions</span></span>

<span data-ttu-id="2d40b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2d40b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d40b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2d40b-108">Permission type</span></span>      | <span data-ttu-id="2d40b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2d40b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d40b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2d40b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2d40b-111">RoleManagement、RoleManagement、Directory.accessasuser.all、all、、all、all 和的所有子目录。</span><span class="sxs-lookup"><span data-stu-id="2d40b-111">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2d40b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2d40b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d40b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d40b-113">Not supported.</span></span>    |
|<span data-ttu-id="2d40b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2d40b-114">Application</span></span> | <span data-ttu-id="2d40b-115">RoleManagement、RoleManagement、目录和所有读写的所有子目录。所有</span><span class="sxs-lookup"><span data-stu-id="2d40b-115">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d40b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2d40b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2d40b-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2d40b-117">Optional query parameters</span></span>

<span data-ttu-id="2d40b-118">此操作需要`$filter`查询参数。</span><span class="sxs-lookup"><span data-stu-id="2d40b-118">This operation requires the `$filter` query parameter.</span></span> <span data-ttu-id="2d40b-119">您可以对`roleDefinitionId`或`principalId`属性进行筛选。</span><span class="sxs-lookup"><span data-stu-id="2d40b-119">You can filter on the `roleDefinitionId` or `principalId` properties.</span></span> <span data-ttu-id="2d40b-120">该`roleDefinitionId`属性可以是角色对象 id, 也可以是角色模板对象 id。</span><span class="sxs-lookup"><span data-stu-id="2d40b-120">The `roleDefinitionId` property can be either a role object ID or a role template object ID.</span></span> <span data-ttu-id="2d40b-121">有关一般信息, 请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="2d40b-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2d40b-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="2d40b-122">Request headers</span></span>

| <span data-ttu-id="2d40b-123">名称</span><span class="sxs-lookup"><span data-stu-id="2d40b-123">Name</span></span>      |<span data-ttu-id="2d40b-124">说明</span><span class="sxs-lookup"><span data-stu-id="2d40b-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2d40b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d40b-125">Authorization</span></span> | <span data-ttu-id="2d40b-126">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="2d40b-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d40b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2d40b-127">Request body</span></span>

<span data-ttu-id="2d40b-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2d40b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d40b-129">响应</span><span class="sxs-lookup"><span data-stu-id="2d40b-129">Response</span></span>

<span data-ttu-id="2d40b-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[unifiedRoleAssignment](../resources/unifiedroleassignment.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="2d40b-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2d40b-131">示例</span><span class="sxs-lookup"><span data-stu-id="2d40b-131">Examples</span></span>

### <a name="example-1-request-using-a-filter-on-role-definition-id"></a><span data-ttu-id="2d40b-132">示例 1: 使用角色定义 ID 的筛选器请求</span><span class="sxs-lookup"><span data-stu-id="2d40b-132">Example 1: Request using a filter on role definition ID</span></span>

#### <a name="request"></a><span data-ttu-id="2d40b-133">请求</span><span class="sxs-lookup"><span data-stu-id="2d40b-133">Request</span></span>

<span data-ttu-id="2d40b-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2d40b-134">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2d40b-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="2d40b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roleAssignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments?$filter=roleDefinitionId eq '62e90394-69f5-4237-9190-012177145e10'
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2d40b-136">C#</span><span class="sxs-lookup"><span data-stu-id="2d40b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2d40b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d40b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2d40b-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="2d40b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2d40b-139">响应</span><span class="sxs-lookup"><span data-stu-id="2d40b-139">Response</span></span>

<span data-ttu-id="2d40b-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2d40b-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments",
    "value": [
        {
            "id": "lAPpYvVpN0KRkAEhdxReEGm3jqnUe4lEhvatluHVi2I-1",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "resourceScope": "/",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10"
        },
        {
            "id": "lAPpYvVpN0KRkAEhdxReEGnbHktRMANMpnGtLZ3MXeY-1",
            "principalId": "4b1edb69-3051-4c03-a671-ad2d9dcc5de6",
            "resourceScope": "/",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10"
        },
        {
            "id": "lAPpYvVpN0KRkAEhdxReEKLh1vKaL9NIi6cTuyyN_6Q-1",
            "principalId": "f2d6e1a2-2f9a-48d3-8ba7-13bb2c8dffa4",
            "resourceScope": "/",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10"
        },
        {
            "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
            "principalId": "4ab0b690-479b-47ff-af8f-2576cf521872",
            "resourceScope": "/",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10"
        },
        {
            "id": "lAPpYvVpN0KRkAEhdxReEGXxIcn3O7hBqaGB0NGuCwE-1",
            "principalId": "c921f165-3bf7-41b8-a9a1-81d0d1ae0b01",
            "resourceScope": "/",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10"
        },
        {
            "id": "lAPpYvVpN0KRkAEhdxReEAWO6-FSXqhEg1mkkLETmA8-1",
            "principalId": "e1eb8e05-5e52-44a8-8359-a490b113980f",
            "resourceScope": "/",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10"
        }
    ]
}
```

### <a name="example-2-request-using-a-filter-on-principal-id"></a><span data-ttu-id="2d40b-141">示例 2: 对主体 ID 使用筛选器请求</span><span class="sxs-lookup"><span data-stu-id="2d40b-141">Example 2: Request using a filter on principal ID</span></span>

#### <a name="request"></a><span data-ttu-id="2d40b-142">请求</span><span class="sxs-lookup"><span data-stu-id="2d40b-142">Request</span></span>

<span data-ttu-id="2d40b-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2d40b-143">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2d40b-144">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="2d40b-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roleAssignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments?$filter=principalId eq 'a98eb769-7bd4-4489-86f6-ad96e1d58b62'
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2d40b-145">C#</span><span class="sxs-lookup"><span data-stu-id="2d40b-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2d40b-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d40b-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2d40b-147">目标-C</span><span class="sxs-lookup"><span data-stu-id="2d40b-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2d40b-148">响应</span><span class="sxs-lookup"><span data-stu-id="2d40b-148">Response</span></span>

<span data-ttu-id="2d40b-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2d40b-149">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments",
    "value": [
        {
            "id": "lAPpYvVpN0KRkAEhdxReEGm3jqnUe4lEhvatluHVi2I-1",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "resourceScope": "/",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10"
        },
        {
            "id": "uBph6InB6EaU4WAhOrH4FGm3jqnUe4lEhvatluHVi2I-1",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "resourceScope": "/",
            "roleDefinitionId": "e8611ab8-c189-46e8-94e1-60213ab1f814"
        },
        {
            "id": "5wuT_mJe20eRr5jDpJo4sWm3jqnUe4lEhvatluHVi2I-1",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "resourceScope": "/",
            "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1"
        },
        {
            "id": "5TgczyE2BECny4eWJNztfGm3jqnUe4lEhvatluHVi2I-1",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "resourceScope": "/",
            "roleDefinitionId": "cf1c38e5-3621-4004-a7cb-879624dced7c"
        },
        {
            "id": "CRCUdVqRaUir52kb_xgnnmm3jqnUe4lEhvatluHVi2I-1",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "resourceScope": "/",
            "roleDefinitionId": "75941009-915a-4869-abe7-691bff18279e"
        },
        {
            "id": "4yeYchSc90m7G5YI8Va7uGm3jqnUe4lEhvatluHVi2I-1",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "resourceScope": "/",
            "roleDefinitionId": "729827e3-9c14-49f7-bb1b-9608f156bbb8"
        },
        {
            "id": "y-RKGSaxskC9W2CRs4CXfWm3jqnUe4lEhvatluHVi2I-1",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "resourceScope": "/",
            "roleDefinitionId": "194ae4cb-b126-40b2-bd5b-6091b380977d"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List roleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
