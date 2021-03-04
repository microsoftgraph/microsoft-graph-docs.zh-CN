---
title: 更新 oAuth2PermissionGrant
description: 更新 oAuth2PermissionGrant 的属性，表示委派的权限授予。
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 0c9d3f60eeff2edd01d6926fb2fed18a3e508db4
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447909"
---
# <a name="update-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="14110-103">更新 oAuth2PermissionGrant (委派) </span><span class="sxs-lookup"><span data-stu-id="14110-103">Update a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="14110-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14110-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="14110-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14110-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14110-106">更新 [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) 对象的属性，表示委派的权限授予。</span><span class="sxs-lookup"><span data-stu-id="14110-106">Update the properties of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object, representing a delegated permission grant.</span></span>

<span data-ttu-id="14110-107">**oAuth2PermissionGrant** 可通过在作用域中添加或删除列表中的项目来更改授予的委派 **权限**。</span><span class="sxs-lookup"><span data-stu-id="14110-107">An **oAuth2PermissionGrant** can be updated to change which delegated permissions are granted, by adding or removing items from the list in **scopes**.</span></span>

## <a name="permissions"></a><span data-ttu-id="14110-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="14110-108">Permissions</span></span>

<span data-ttu-id="14110-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="14110-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14110-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="14110-111">Permission type</span></span>      | <span data-ttu-id="14110-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="14110-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14110-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="14110-113">Delegated (work or school account)</span></span> | <span data-ttu-id="14110-114">DelegatedPermissionGrant.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="14110-114">DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="14110-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="14110-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14110-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="14110-116">Not supported.</span></span>    |
|<span data-ttu-id="14110-117">Application</span><span class="sxs-lookup"><span data-stu-id="14110-117">Application</span></span> | <span data-ttu-id="14110-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14110-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="14110-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="14110-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /oauth2PermissionGrants/{id}
```

## <a name="request-headers"></a><span data-ttu-id="14110-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="14110-120">Request headers</span></span>

| <span data-ttu-id="14110-121">名称</span><span class="sxs-lookup"><span data-stu-id="14110-121">Name</span></span>       | <span data-ttu-id="14110-122">类型</span><span class="sxs-lookup"><span data-stu-id="14110-122">Type</span></span> | <span data-ttu-id="14110-123">说明</span><span class="sxs-lookup"><span data-stu-id="14110-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="14110-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="14110-124">Authorization</span></span>  | <span data-ttu-id="14110-125">string</span><span class="sxs-lookup"><span data-stu-id="14110-125">string</span></span>  | <span data-ttu-id="14110-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="14110-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14110-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="14110-128">Request body</span></span>

<span data-ttu-id="14110-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="14110-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="14110-132">属性</span><span class="sxs-lookup"><span data-stu-id="14110-132">Property</span></span>     | <span data-ttu-id="14110-133">类型</span><span class="sxs-lookup"><span data-stu-id="14110-133">Type</span></span>   |<span data-ttu-id="14110-134">说明</span><span class="sxs-lookup"><span data-stu-id="14110-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="14110-135">scope</span><span class="sxs-lookup"><span data-stu-id="14110-135">scope</span></span>|<span data-ttu-id="14110-136">String</span><span class="sxs-lookup"><span data-stu-id="14110-136">String</span></span>| <span data-ttu-id="14110-137">指定资源应用程序应在 OAuth 2.0 访问令牌中预期的范围声明的值。</span><span class="sxs-lookup"><span data-stu-id="14110-137">Specifies the value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="response"></a><span data-ttu-id="14110-138">响应</span><span class="sxs-lookup"><span data-stu-id="14110-138">Response</span></span>

<span data-ttu-id="14110-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="14110-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14110-141">示例</span><span class="sxs-lookup"><span data-stu-id="14110-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="14110-142">请求</span><span class="sxs-lookup"><span data-stu-id="14110-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="14110-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="14110-143">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "update_oAuth2PermissionGrant"
}-->

```http
PATCH https://graph.microsoft.com/beta/oauth2PermissionGrants/{id}
Content-Type: application/json
Content-Length: 30

{
  "scope": "scope-value"
}
```

# <a name="c"></a>[<span data-ttu-id="14110-144">C#</span><span class="sxs-lookup"><span data-stu-id="14110-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14110-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14110-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14110-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14110-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="14110-147">Java</span><span class="sxs-lookup"><span data-stu-id="14110-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-oauth2permissiongrant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="14110-148">响应</span><span class="sxs-lookup"><span data-stu-id="14110-148">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update oAuth2PermissionGrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


