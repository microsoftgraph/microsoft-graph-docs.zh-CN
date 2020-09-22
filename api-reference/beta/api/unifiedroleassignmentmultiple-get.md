---
title: 获取 unifiedRoleAssignmentMultiple
description: 检索 unifiedRoleAssignmentMultiple 对象的属性和关系。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0b4300a3f5256b69b24c5df53866d970e0858b88
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989890"
---
# <a name="get-unifiedroleassignmentmultiple"></a><span data-ttu-id="e931b-103">获取 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="e931b-103">Get unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="e931b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e931b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e931b-105">检索 [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e931b-105">Retrieve the properties and relationships of a [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="e931b-106">使用此对象可在 Microsoft Intune 中获取角色分配。</span><span class="sxs-lookup"><span data-stu-id="e931b-106">Use this object for get role assignments in Microsoft Intune.</span></span> <span data-ttu-id="e931b-107">对于其他 Micrsoft 365 应用程序 (如 Azure AD) ，请使用 [unifiedRoleAssignment](../resources/unifiedroleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="e931b-107">For other Micrsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e931b-108">权限</span><span class="sxs-lookup"><span data-stu-id="e931b-108">Permissions</span></span>

<span data-ttu-id="e931b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e931b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e931b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e931b-111">Permission type</span></span> | <span data-ttu-id="e931b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e931b-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="e931b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e931b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e931b-114">Devicemanagementrbac.readwrite.all、Devicemanagementrbac.readwrite.all 和所有</span><span class="sxs-lookup"><span data-stu-id="e931b-114">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="e931b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e931b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e931b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e931b-116">Not supported.</span></span> |
| <span data-ttu-id="e931b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e931b-117">Application</span></span> | <span data-ttu-id="e931b-118">Devicemanagementrbac.readwrite.all、Devicemanagementrbac.readwrite.all 和所有</span><span class="sxs-lookup"><span data-stu-id="e931b-118">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e931b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e931b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/deviceManagement/roleAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e931b-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e931b-120">Optional query parameters</span></span>

<span data-ttu-id="e931b-121">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e931b-121">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="e931b-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="e931b-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e931b-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="e931b-123">Request headers</span></span>

| <span data-ttu-id="e931b-124">名称</span><span class="sxs-lookup"><span data-stu-id="e931b-124">Name</span></span>  | <span data-ttu-id="e931b-125">说明</span><span class="sxs-lookup"><span data-stu-id="e931b-125">Description</span></span> |
|:----- |:----------- |
| <span data-ttu-id="e931b-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e931b-126">Authorization</span></span> | <span data-ttu-id="e931b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e931b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e931b-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="e931b-129">Request body</span></span>

<span data-ttu-id="e931b-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e931b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e931b-131">响应</span><span class="sxs-lookup"><span data-stu-id="e931b-131">Response</span></span>

<span data-ttu-id="e931b-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e931b-132">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e931b-133">示例</span><span class="sxs-lookup"><span data-stu-id="e931b-133">Examples</span></span>

### <a name="example-1-get-a-directory-scoped-roleassignmentmultiple-in-intune"></a><span data-ttu-id="e931b-134">示例1：在 Intune 中获取目录范围的 roleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="e931b-134">Example 1: Get a directory-scoped roleAssignmentMultiple in Intune</span></span>

#### <a name="request"></a><span data-ttu-id="e931b-135">请求</span><span class="sxs-lookup"><span data-stu-id="e931b-135">Request</span></span>

<span data-ttu-id="e931b-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e931b-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e931b-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="e931b-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentmultiple"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="e931b-138">C#</span><span class="sxs-lookup"><span data-stu-id="e931b-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignmentmultiple-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e931b-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e931b-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignmentmultiple-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e931b-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e931b-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignmentmultiple-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e931b-141">响应</span><span class="sxs-lookup"><span data-stu-id="e931b-141">Response</span></span>

<span data-ttu-id="e931b-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e931b-142">The following is an example of the response.</span></span>
> <span data-ttu-id="e931b-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e931b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-roleassignmentmultiple-in-intune-assigned-to-a-group"></a><span data-ttu-id="e931b-145">示例2：在分配给组的 Intune 中获取 roleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="e931b-145">Example 2: Get a roleAssignmentMultiple in Intune assigned to a group</span></span>

#### <a name="request"></a><span data-ttu-id="e931b-146">请求</span><span class="sxs-lookup"><span data-stu-id="e931b-146">Request</span></span>

<span data-ttu-id="e931b-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e931b-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e931b-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="e931b-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentmultiple"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments?$filter = principalIds/any(x:x eq '564ae70c-73d9-476b-820b-fb61eb7384b9')
```
# <a name="c"></a>[<span data-ttu-id="e931b-149">C#</span><span class="sxs-lookup"><span data-stu-id="e931b-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignmentmultiple-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e931b-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e931b-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignmentmultiple-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e931b-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e931b-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignmentmultiple-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e931b-152">响应</span><span class="sxs-lookup"><span data-stu-id="e931b-152">Response</span></span>

<span data-ttu-id="e931b-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e931b-153">The following is an example of the response.</span></span>
> <span data-ttu-id="e931b-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e931b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-get-a-directory-scoped-roleassignmentmultiple-with-expand"></a><span data-ttu-id="e931b-156">示例3：获取目录范围的 roleAssignmentMultiple `$expand`</span><span class="sxs-lookup"><span data-stu-id="e931b-156">Example 3: Get a directory-scoped roleAssignmentMultiple with `$expand`</span></span>

#### <a name="request"></a><span data-ttu-id="e931b-157">请求</span><span class="sxs-lookup"><span data-stu-id="e931b-157">Request</span></span>

<span data-ttu-id="e931b-158">以下是包含查询参数的请求的示例 `$expand` 。</span><span class="sxs-lookup"><span data-stu-id="e931b-158">The following is an example of the request with the `$expand` query parameter.</span></span>


# <a name="http"></a>[<span data-ttu-id="e931b-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="e931b-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1?$expand=roleDefinition,principals,directoryScopes
```
# <a name="c"></a>[<span data-ttu-id="e931b-160">C#</span><span class="sxs-lookup"><span data-stu-id="e931b-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e931b-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e931b-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e931b-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e931b-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e931b-163">响应</span><span class="sxs-lookup"><span data-stu-id="e931b-163">Response</span></span>

<span data-ttu-id="e931b-164">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e931b-164">The following is an example of the response.</span></span>
> <span data-ttu-id="e931b-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e931b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


