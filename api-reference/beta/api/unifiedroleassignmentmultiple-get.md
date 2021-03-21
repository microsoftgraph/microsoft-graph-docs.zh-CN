---
title: 获取 unifiedRoleAssignmentMultiple
description: 检索 unifiedRoleAssignmentMultiple 对象的属性和关系。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 9e9867d2c314534115f7c620d52329805d8b890e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960574"
---
# <a name="get-unifiedroleassignmentmultiple"></a><span data-ttu-id="55d22-103">获取 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="55d22-103">Get unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="55d22-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55d22-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55d22-105">检索 [unifiedRoleAssignmentMultiple 对象的属性和](../resources/unifiedroleassignmentmultiple.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="55d22-105">Retrieve the properties and relationships of a [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="55d22-106">使用此对象获取 Microsoft Intune 中的角色分配。</span><span class="sxs-lookup"><span data-stu-id="55d22-106">Use this object for get role assignments in Microsoft Intune.</span></span> <span data-ttu-id="55d22-107">对于 Azure AD (等其他 Microsoft 365) ，请使用 [unifiedRoleAssignment](../resources/unifiedroleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="55d22-107">For other Microsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="55d22-108">权限</span><span class="sxs-lookup"><span data-stu-id="55d22-108">Permissions</span></span>

<span data-ttu-id="55d22-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="55d22-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="55d22-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="55d22-111">Permission type</span></span> | <span data-ttu-id="55d22-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="55d22-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="55d22-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="55d22-113">Delegated (work or school account)</span></span> | <span data-ttu-id="55d22-114">DeviceManagementRBAC.Read.All、DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55d22-114">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="55d22-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="55d22-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55d22-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="55d22-116">Not supported.</span></span> |
| <span data-ttu-id="55d22-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="55d22-117">Application</span></span> | <span data-ttu-id="55d22-118">DeviceManagementRBAC.Read.All、DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55d22-118">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="55d22-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="55d22-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/deviceManagement/roleAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="55d22-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="55d22-120">Optional query parameters</span></span>

<span data-ttu-id="55d22-121">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="55d22-121">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="55d22-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="55d22-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="55d22-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="55d22-123">Request headers</span></span>

| <span data-ttu-id="55d22-124">名称</span><span class="sxs-lookup"><span data-stu-id="55d22-124">Name</span></span>  | <span data-ttu-id="55d22-125">说明</span><span class="sxs-lookup"><span data-stu-id="55d22-125">Description</span></span> |
|:----- |:----------- |
| <span data-ttu-id="55d22-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="55d22-126">Authorization</span></span> | <span data-ttu-id="55d22-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="55d22-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55d22-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="55d22-129">Request body</span></span>

<span data-ttu-id="55d22-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="55d22-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55d22-131">响应</span><span class="sxs-lookup"><span data-stu-id="55d22-131">Response</span></span>

<span data-ttu-id="55d22-132">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="55d22-132">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="55d22-133">示例</span><span class="sxs-lookup"><span data-stu-id="55d22-133">Examples</span></span>

### <a name="example-1-get-a-directory-scoped-roleassignmentmultiple-in-intune"></a><span data-ttu-id="55d22-134">示例 1：在 Intune 中获取目录作用域角色AssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="55d22-134">Example 1: Get a directory-scoped roleAssignmentMultiple in Intune</span></span>

#### <a name="request"></a><span data-ttu-id="55d22-135">请求</span><span class="sxs-lookup"><span data-stu-id="55d22-135">Request</span></span>

<span data-ttu-id="55d22-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="55d22-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="55d22-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="55d22-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentmultiple_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="55d22-138">C#</span><span class="sxs-lookup"><span data-stu-id="55d22-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignmentmultiple-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55d22-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55d22-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignmentmultiple-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55d22-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55d22-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignmentmultiple-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="55d22-141">Java</span><span class="sxs-lookup"><span data-stu-id="55d22-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignmentmultiple-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="55d22-142">响应</span><span class="sxs-lookup"><span data-stu-id="55d22-142">Response</span></span>

<span data-ttu-id="55d22-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="55d22-143">The following is an example of the response.</span></span>
> <span data-ttu-id="55d22-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="55d22-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/deviceManagement/roleAssignments/$entity",
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
    "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
    "principalIds[]": ["4ab0b690-479b-47ff-af8f-2576cf521872", "f8ca5a85-489a-49a0-b555-0a6d81e56f0d"],
    "directoryScopeIds[]": ["28ca5a85-489a-49a0-b555-0a6d81e56f0", "8152656a-cf9a-4928-a457-1512d4cae295"]
}
```

### <a name="example-2-get-a-roleassignmentmultiple-in-intune-assigned-to-a-group"></a><span data-ttu-id="55d22-146">示例 2：获取分配给组的 Intune 中的 roleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="55d22-146">Example 2: Get a roleAssignmentMultiple in Intune assigned to a group</span></span>

#### <a name="request"></a><span data-ttu-id="55d22-147">请求</span><span class="sxs-lookup"><span data-stu-id="55d22-147">Request</span></span>

<span data-ttu-id="55d22-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="55d22-148">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="55d22-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="55d22-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentmultiple_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments?$filter = principalIds/any(x:x eq '564ae70c-73d9-476b-820b-fb61eb7384b9')
```
# <a name="c"></a>[<span data-ttu-id="55d22-150">C#</span><span class="sxs-lookup"><span data-stu-id="55d22-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignmentmultiple-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55d22-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55d22-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignmentmultiple-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55d22-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55d22-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignmentmultiple-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="55d22-153">Java</span><span class="sxs-lookup"><span data-stu-id="55d22-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignmentmultiple-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="55d22-154">响应</span><span class="sxs-lookup"><span data-stu-id="55d22-154">Response</span></span>

<span data-ttu-id="55d22-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="55d22-155">The following is an example of the response.</span></span>
> <span data-ttu-id="55d22-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="55d22-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/deviceManagement/roleAssignments",
    "@odata.count": 7,
    "value": [
        {
            "id": "893fc648-73fc-482b-b964-ddd1cabf0db4",
            "condition": null,
            "displayName": "Assign Contoso_App_Admin to School Admin",
            "description": "test",
            "roleDefinitionId": "2f9f4f7e-2d13-427b-adf2-361a1eef7ae8",
            "principalIds": [
                "564ae70c-73d9-476b-820b-fb61eb7384b9"
            ],
            "directoryScopeIds": [],
            "appScopeIds": [
                "0",
                "AllLicensedUsers"
            ]
        }
    ]
}
```

### <a name="example-3-get-a-directory-scoped-roleassignmentmultiple-with-expand"></a><span data-ttu-id="55d22-158">示例 3：使用 获取目录作用域角色AssignmentMultiple `$expand`</span><span class="sxs-lookup"><span data-stu-id="55d22-158">Example 3: Get a directory-scoped roleAssignmentMultiple with `$expand`</span></span>

#### <a name="request"></a><span data-ttu-id="55d22-159">请求</span><span class="sxs-lookup"><span data-stu-id="55d22-159">Request</span></span>

<span data-ttu-id="55d22-160">下面是一个包含查询参数 `$expand` 的请求示例。</span><span class="sxs-lookup"><span data-stu-id="55d22-160">The following is an example of the request with the `$expand` query parameter.</span></span>


# <a name="http"></a>[<span data-ttu-id="55d22-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="55d22-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_3"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1?$expand=roleDefinition,principals,directoryScopes
```
# <a name="c"></a>[<span data-ttu-id="55d22-162">C#</span><span class="sxs-lookup"><span data-stu-id="55d22-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55d22-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55d22-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55d22-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55d22-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="55d22-165">Java</span><span class="sxs-lookup"><span data-stu-id="55d22-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="55d22-166">响应</span><span class="sxs-lookup"><span data-stu-id="55d22-166">Response</span></span>

<span data-ttu-id="55d22-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="55d22-167">The following is an example of the response.</span></span>
> <span data-ttu-id="55d22-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="55d22-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/deviceManagement/roleAssignments/$entity",
  "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
  "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
  "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
  "roleDefinition": {
    "id": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "displayName": "Application Manager",
    "description": "Manages mobile and managed applications",
    "rolePermissions": [
      {
        "allowedResourceActions": [],
        "excludedResourceActions": [],
    }],
    "isEnabled": true,
    "isBuiltIn": true,
  },
  "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
  "principals": [
    {
      "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
      "id": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
      "displayName": "Global IT"
    },
    {
      "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
      "id": "c1518aa9-4da5-4c84-a902-a31404023890",
      "displayName": "Americas IT"
    }
],
  "directoryScopeIds": ["28ca5a85-489a-49a0-b555-0a6d81e56f0d", "8152656a-cf9a-4928-a457-1512d4cae295"],
  "directoryScopes": [
    {
      "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
      "id": "28ca5a85-489a-49a0-b555-0a6d81e56f0d",
      "displayName": "Washington Sales Region"
    },
    {
      "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
      "id": "8152656a-cf9a-4928-a457-1512d4cae295",
      "displayName": "Oregon Sales Region"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get unifiedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


