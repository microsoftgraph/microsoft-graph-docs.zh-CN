---
title: 更新 oAuth2PermissionGrant
description: 更新 oAuth2PermissionGrant 的属性，该属性代表委派权限授予。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: f7e71b2ce52eda50008ceb7499981423acdbc424
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335259"
---
# <a name="update-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="8dede-103">更新委派权限授予（oAuth2PermissionGrant）</span><span class="sxs-lookup"><span data-stu-id="8dede-103">Update a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="8dede-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8dede-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="8dede-105">更新[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md)对象的属性，该对象代表委派权限授予。</span><span class="sxs-lookup"><span data-stu-id="8dede-105">Update the properties of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object, representing a delegated permission grant.</span></span>

<span data-ttu-id="8dede-106">可以通过在**范围**的列表中添加或删除项目来更新**oAuth2PermissionGrant** ，以更改要授予的委派权限。</span><span class="sxs-lookup"><span data-stu-id="8dede-106">An **oAuth2PermissionGrant** can be updated to change which delegated permissions are granted, by adding or removing items from the list in **scopes**.</span></span>

## <a name="permissions"></a><span data-ttu-id="8dede-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="8dede-107">Permissions</span></span>

<span data-ttu-id="8dede-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8dede-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8dede-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8dede-110">Permission type</span></span>      | <span data-ttu-id="8dede-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8dede-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8dede-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8dede-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8dede-113">DelegatedPermissionGrant、Directory.accessasuser.all、all 和的所有子目录</span><span class="sxs-lookup"><span data-stu-id="8dede-113">DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8dede-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8dede-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8dede-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8dede-115">Not supported.</span></span>    |
|<span data-ttu-id="8dede-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8dede-116">Application</span></span> | <span data-ttu-id="8dede-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dede-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8dede-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8dede-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /oauth2PermissionGrants/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8dede-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8dede-119">Request headers</span></span>

| <span data-ttu-id="8dede-120">名称</span><span class="sxs-lookup"><span data-stu-id="8dede-120">Name</span></span>       | <span data-ttu-id="8dede-121">类型</span><span class="sxs-lookup"><span data-stu-id="8dede-121">Type</span></span> | <span data-ttu-id="8dede-122">说明</span><span class="sxs-lookup"><span data-stu-id="8dede-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8dede-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8dede-123">Authorization</span></span>  | <span data-ttu-id="8dede-124">string</span><span class="sxs-lookup"><span data-stu-id="8dede-124">string</span></span>  | <span data-ttu-id="8dede-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8dede-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8dede-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8dede-127">Request body</span></span>

<span data-ttu-id="8dede-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="8dede-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8dede-131">属性</span><span class="sxs-lookup"><span data-stu-id="8dede-131">Property</span></span>     | <span data-ttu-id="8dede-132">类型</span><span class="sxs-lookup"><span data-stu-id="8dede-132">Type</span></span>   |<span data-ttu-id="8dede-133">Description</span><span class="sxs-lookup"><span data-stu-id="8dede-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8dede-134">scope</span><span class="sxs-lookup"><span data-stu-id="8dede-134">scope</span></span>|<span data-ttu-id="8dede-135">String</span><span class="sxs-lookup"><span data-stu-id="8dede-135">String</span></span>| <span data-ttu-id="8dede-136">指定在 OAuth 2.0 访问令牌中，资源应用程序应预期的范围声明的值。</span><span class="sxs-lookup"><span data-stu-id="8dede-136">Specifies the value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="response"></a><span data-ttu-id="8dede-137">响应</span><span class="sxs-lookup"><span data-stu-id="8dede-137">Response</span></span>

<span data-ttu-id="8dede-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8dede-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8dede-140">示例</span><span class="sxs-lookup"><span data-stu-id="8dede-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="8dede-141">请求</span><span class="sxs-lookup"><span data-stu-id="8dede-141">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8dede-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="8dede-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_oAuth2PermissionGrant"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/oauth2PermissionGrants/{id}
Content-Type: application/json
Content-Length: 30

{
  "scope": "scope-value"
}
```
# <a name="c"></a>[<span data-ttu-id="8dede-143">C#</span><span class="sxs-lookup"><span data-stu-id="8dede-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8dede-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8dede-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8dede-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8dede-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8dede-146">Java</span><span class="sxs-lookup"><span data-stu-id="8dede-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-oauth2permissiongrant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8dede-147">响应</span><span class="sxs-lookup"><span data-stu-id="8dede-147">Response</span></span>

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
