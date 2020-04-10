---
title: 列出 unifiedRoleAssignments
description: 获取 unifiedRoleAssignment 对象的列表。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dba161cbfbf6b14f477e9f156858b59d555833b7
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43216857"
---
# <a name="list-unifiedroleassignments"></a><span data-ttu-id="ddc91-103">列出 unifiedRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="ddc91-103">List unifiedRoleAssignments</span></span>

<span data-ttu-id="ddc91-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddc91-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddc91-105">获取提供程序的[unifiedRoleAssignment](../resources/unifiedroleassignment.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="ddc91-105">Get a list of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) objects for the provider.</span></span>

## <a name="permissions"></a><span data-ttu-id="ddc91-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="ddc91-106">Permissions</span></span>

<span data-ttu-id="ddc91-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ddc91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddc91-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ddc91-109">Permission type</span></span>      | <span data-ttu-id="ddc91-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ddc91-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ddc91-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ddc91-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ddc91-112">RoleManagement、RoleManagement、Directory.accessasuser.all、all、、all、all 和的所有子目录。</span><span class="sxs-lookup"><span data-stu-id="ddc91-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ddc91-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ddc91-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddc91-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ddc91-114">Not supported.</span></span>    |
|<span data-ttu-id="ddc91-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ddc91-115">Application</span></span> | <span data-ttu-id="ddc91-116">RoleManagement、RoleManagement、目录和所有读写的所有子目录。所有</span><span class="sxs-lookup"><span data-stu-id="ddc91-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ddc91-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ddc91-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ddc91-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ddc91-118">Optional query parameters</span></span>

<span data-ttu-id="ddc91-119">此操作需要`$filter`查询参数。</span><span class="sxs-lookup"><span data-stu-id="ddc91-119">This operation requires the `$filter` query parameter.</span></span> <span data-ttu-id="ddc91-120">您可以对`roleDefinitionId`或`principalId`属性进行筛选。</span><span class="sxs-lookup"><span data-stu-id="ddc91-120">You can filter on the `roleDefinitionId` or `principalId` properties.</span></span> <span data-ttu-id="ddc91-121">该`roleDefinitionId`属性可以是角色对象 id，也可以是角色模板对象 id。</span><span class="sxs-lookup"><span data-stu-id="ddc91-121">The `roleDefinitionId` property can be either a role object ID or a role template object ID.</span></span> <span data-ttu-id="ddc91-122">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="ddc91-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ddc91-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="ddc91-123">Request headers</span></span>

| <span data-ttu-id="ddc91-124">名称</span><span class="sxs-lookup"><span data-stu-id="ddc91-124">Name</span></span>      |<span data-ttu-id="ddc91-125">说明</span><span class="sxs-lookup"><span data-stu-id="ddc91-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ddc91-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddc91-126">Authorization</span></span> | <span data-ttu-id="ddc91-127">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="ddc91-127">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ddc91-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ddc91-128">Request body</span></span>

<span data-ttu-id="ddc91-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ddc91-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddc91-130">响应</span><span class="sxs-lookup"><span data-stu-id="ddc91-130">Response</span></span>

<span data-ttu-id="ddc91-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[unifiedRoleAssignment](../resources/unifiedroleassignment.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="ddc91-131">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ddc91-132">示例</span><span class="sxs-lookup"><span data-stu-id="ddc91-132">Examples</span></span>

### <a name="example-1-request-using-a-filter-on-role-definition-id"></a><span data-ttu-id="ddc91-133">示例1：使用角色定义 ID 的筛选器请求</span><span class="sxs-lookup"><span data-stu-id="ddc91-133">Example 1: Request using a filter on role definition ID</span></span>

#### <a name="request"></a><span data-ttu-id="ddc91-134">请求</span><span class="sxs-lookup"><span data-stu-id="ddc91-134">Request</span></span>

<span data-ttu-id="ddc91-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ddc91-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ddc91-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddc91-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roleAssignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments?$filter=roleDefinitionId eq '62e90394-69f5-4237-9190-012177145e10'
```
# <a name="c"></a>[<span data-ttu-id="ddc91-137">C#</span><span class="sxs-lookup"><span data-stu-id="ddc91-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ddc91-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddc91-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ddc91-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ddc91-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ddc91-140">响应</span><span class="sxs-lookup"><span data-stu-id="ddc91-140">Response</span></span>

<span data-ttu-id="ddc91-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ddc91-141">The following is an example of the response.</span></span>

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
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "lAPpYvVpN0KRkAEhdxReEGm3jqnUe4lEhvatluHVi2I-1",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "directoryScopeId": "/"
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "lAPpYvVpN0KRkAEhdxReEGnbHktRMANMpnGtLZ3MXeY-1",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principalId": "4b1edb69-3051-4c03-a671-ad2d9dcc5de6",
            "directoryScopeId": "/"
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "lAPpYvVpN0KRkAEhdxReEKLh1vKaL9NIi6cTuyyN_6Q-1",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principalId": "f2d6e1a2-2f9a-48d3-8ba7-13bb2c8dffa4",
            "directoryScopeId": "/"
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principalId": "4ab0b690-479b-47ff-af8f-2576cf521872",
            "directoryScopeId": "/"
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "lAPpYvVpN0KRkAEhdxReEGXxIcn3O7hBqaGB0NGuCwE-1",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principalId": "c921f165-3bf7-41b8-a9a1-81d0d1ae0b01",
            "directoryScopeId": "/"
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "lAPpYvVpN0KRkAEhdxReEAWO6-FSXqhEg1mkkLETmA8-1",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principalId": "e1eb8e05-5e52-44a8-8359-a490b113980f",
            "directoryScopeId": "/"
        }
    ]
}
```

### <a name="example-2-request-using-a-filter-on-principal-id"></a><span data-ttu-id="ddc91-142">示例2：对主体 ID 使用筛选器请求</span><span class="sxs-lookup"><span data-stu-id="ddc91-142">Example 2: Request using a filter on principal ID</span></span>

#### <a name="request"></a><span data-ttu-id="ddc91-143">请求</span><span class="sxs-lookup"><span data-stu-id="ddc91-143">Request</span></span>

<span data-ttu-id="ddc91-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ddc91-144">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ddc91-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddc91-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roleAssignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments?$filter=principalId eq 'a98eb769-7bd4-4489-86f6-ad96e1d58b62'
```
# <a name="c"></a>[<span data-ttu-id="ddc91-146">C#</span><span class="sxs-lookup"><span data-stu-id="ddc91-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ddc91-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddc91-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ddc91-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ddc91-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ddc91-149">响应</span><span class="sxs-lookup"><span data-stu-id="ddc91-149">Response</span></span>

<span data-ttu-id="ddc91-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ddc91-150">The following is an example of the response.</span></span>

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
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "lAPpYvVpN0KRkAEhdxReEGm3jqnUe4lEhvatluHVi2I-1",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "directoryScopeId": "/"            
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "uBph6InB6EaU4WAhOrH4FGm3jqnUe4lEhvatluHVi2I-1",
            "roleDefinitionId": "e8611ab8-c189-46e8-94e1-60213ab1f814",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "directoryScopeId": "/"            
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "5wuT_mJe20eRr5jDpJo4sWm3jqnUe4lEhvatluHVi2I-1",
            "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "directoryScopeId": "/"            
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "5TgczyE2BECny4eWJNztfGm3jqnUe4lEhvatluHVi2I-1",
            "roleDefinitionId": "cf1c38e5-3621-4004-a7cb-879624dced7c",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "directoryScopeId": "/"            
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "CRCUdVqRaUir52kb_xgnnmm3jqnUe4lEhvatluHVi2I-1",
            "roleDefinitionId": "75941009-915a-4869-abe7-691bff18279e",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "directoryScopeId": "/"            
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "4yeYchSc90m7G5YI8Va7uGm3jqnUe4lEhvatluHVi2I-1",
            "roleDefinitionId": "729827e3-9c14-49f7-bb1b-9608f156bbb8",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "directoryScopeId": "/"            
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
            "id": "y-RKGSaxskC9W2CRs4CXfWm3jqnUe4lEhvatluHVi2I-1",
            "roleDefinitionId": "194ae4cb-b126-40b2-bd5b-6091b380977d",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "directoryScopeId": "/"
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
