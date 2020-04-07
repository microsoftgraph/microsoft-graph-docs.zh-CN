---
title: 获取 unifiedRoleAssignmentMultiple
description: 检索 unifiedRoleAssignmentMultiple 对象的属性和关系。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bffb13cb6c08ddc5d7552d0af3343d4311f6d447
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "43160344"
---
# <a name="get-unifiedroleassignmentmultiple"></a><span data-ttu-id="4bfb5-103">获取 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="4bfb5-103">Get unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="4bfb5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4bfb5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bfb5-105">检索[unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4bfb5-105">Retrieve the properties and relationships of a [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="4bfb5-106">使用此对象可在 Microsoft Intune 中获取角色分配。</span><span class="sxs-lookup"><span data-stu-id="4bfb5-106">Use this object for get role assignments in Microsoft Intune.</span></span> <span data-ttu-id="4bfb5-107">对于其他 Micrsoft 365 应用程序（如 Azure AD），请使用[unifiedRoleAssignment](../resources/unifiedroleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="4bfb5-107">For other Micrsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4bfb5-108">权限</span><span class="sxs-lookup"><span data-stu-id="4bfb5-108">Permissions</span></span>

<span data-ttu-id="4bfb5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4bfb5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4bfb5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4bfb5-111">Permission type</span></span> | <span data-ttu-id="4bfb5-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4bfb5-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="4bfb5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4bfb5-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4bfb5-114">RoleManagement、RoleManagement、Directory.accessasuser.all、all、、all、all 和的所有子目录。</span><span class="sxs-lookup"><span data-stu-id="4bfb5-114">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="4bfb5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4bfb5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bfb5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4bfb5-116">Not supported.</span></span> |
| <span data-ttu-id="4bfb5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4bfb5-117">Application</span></span> | <span data-ttu-id="4bfb5-118">RoleManagement、RoleManagement、目录和所有读写的所有子目录。所有</span><span class="sxs-lookup"><span data-stu-id="4bfb5-118">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4bfb5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4bfb5-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/deviceManagement/roleAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4bfb5-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4bfb5-120">Optional query parameters</span></span>

<span data-ttu-id="4bfb5-121">此方法支持 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4bfb5-121">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="4bfb5-122">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="4bfb5-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4bfb5-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="4bfb5-123">Request headers</span></span>

| <span data-ttu-id="4bfb5-124">名称</span><span class="sxs-lookup"><span data-stu-id="4bfb5-124">Name</span></span>  | <span data-ttu-id="4bfb5-125">说明</span><span class="sxs-lookup"><span data-stu-id="4bfb5-125">Description</span></span> |
|:----- |:----------- |
| <span data-ttu-id="4bfb5-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bfb5-126">Authorization</span></span> | <span data-ttu-id="4bfb5-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4bfb5-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4bfb5-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="4bfb5-129">Request body</span></span>

<span data-ttu-id="4bfb5-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4bfb5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4bfb5-131">响应</span><span class="sxs-lookup"><span data-stu-id="4bfb5-131">Response</span></span>

<span data-ttu-id="4bfb5-132">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4bfb5-132">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4bfb5-133">示例</span><span class="sxs-lookup"><span data-stu-id="4bfb5-133">Examples</span></span>

### <a name="example-1-get-a-directory-scoped-roleassignmentmultiple-in-intune"></a><span data-ttu-id="4bfb5-134">示例1：在 Intune 中获取目录范围的 roleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="4bfb5-134">Example 1: Get a directory-scoped roleAssignmentMultiple in Intune</span></span>

#### <a name="request"></a><span data-ttu-id="4bfb5-135">请求</span><span class="sxs-lookup"><span data-stu-id="4bfb5-135">Request</span></span>

<span data-ttu-id="4bfb5-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4bfb5-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentmultiple"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```

#### <a name="response"></a><span data-ttu-id="4bfb5-137">响应</span><span class="sxs-lookup"><span data-stu-id="4bfb5-137">Response</span></span>

<span data-ttu-id="4bfb5-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4bfb5-138">The following is an example of the response.</span></span>
> <span data-ttu-id="4bfb5-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4bfb5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-directory-scoped-roleassignmentmultiple-with-expand"></a><span data-ttu-id="4bfb5-141">示例2：获取目录范围的 roleAssignmentMultiple`$expand`</span><span class="sxs-lookup"><span data-stu-id="4bfb5-141">Example 2: Get a directory-scoped roleAssignmentMultiple with `$expand`</span></span>

#### <a name="request"></a><span data-ttu-id="4bfb5-142">请求</span><span class="sxs-lookup"><span data-stu-id="4bfb5-142">Request</span></span>

<span data-ttu-id="4bfb5-143">以下是包含`$expand`查询参数的请求的示例。</span><span class="sxs-lookup"><span data-stu-id="4bfb5-143">The following is an example of the request with the `$expand` query parameter.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1?$expand=roleDefinition,principals,directoryScopes
```

#### <a name="response"></a><span data-ttu-id="4bfb5-144">响应</span><span class="sxs-lookup"><span data-stu-id="4bfb5-144">Response</span></span>

<span data-ttu-id="4bfb5-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4bfb5-145">The following is an example of the response.</span></span>
> <span data-ttu-id="4bfb5-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4bfb5-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
