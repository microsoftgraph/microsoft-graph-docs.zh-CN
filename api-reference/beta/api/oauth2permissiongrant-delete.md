---
title: 删除 oAuth2PermissionGrant
description: 删除 oAuth2PermissionGrant。
localization_priority: Normal
ms.openlocfilehash: 1648a706bf27d9bce7de4224f2c6cad32d5660d5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35450084"
---
# <a name="delete-oauth2permissiongrant"></a><span data-ttu-id="c0fb4-103">删除 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="c0fb4-103">Delete oAuth2PermissionGrant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0fb4-104">删除 oAuth2PermissionGrant。</span><span class="sxs-lookup"><span data-stu-id="c0fb4-104">Delete an oAuth2PermissionGrant.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0fb4-105">权限</span><span class="sxs-lookup"><span data-stu-id="c0fb4-105">Permissions</span></span>
<span data-ttu-id="c0fb4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c0fb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c0fb4-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c0fb4-108">Permission type</span></span>      | <span data-ttu-id="c0fb4-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c0fb4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0fb4-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0fb4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c0fb4-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c0fb4-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c0fb4-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c0fb4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0fb4-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0fb4-113">Not supported.</span></span>    |
|<span data-ttu-id="c0fb4-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c0fb4-114">Application</span></span> | <span data-ttu-id="c0fb4-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0fb4-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0fb4-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0fb4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /oAuth2Permissiongrants/{id}
DELETE /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
DELETE /drive/root/createdByUser/oAuth2Permissiongrants/{id}

```
## <a name="request-headers"></a><span data-ttu-id="c0fb4-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0fb4-117">Request headers</span></span>
| <span data-ttu-id="c0fb4-118">名称</span><span class="sxs-lookup"><span data-stu-id="c0fb4-118">Name</span></span>       | <span data-ttu-id="c0fb4-119">类型</span><span class="sxs-lookup"><span data-stu-id="c0fb4-119">Type</span></span> | <span data-ttu-id="c0fb4-120">说明</span><span class="sxs-lookup"><span data-stu-id="c0fb4-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c0fb4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0fb4-121">Authorization</span></span>  | <span data-ttu-id="c0fb4-122">string</span><span class="sxs-lookup"><span data-stu-id="c0fb4-122">string</span></span>  | <span data-ttu-id="c0fb4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c0fb4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0fb4-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0fb4-125">Request body</span></span>
<span data-ttu-id="c0fb4-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c0fb4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0fb4-127">响应</span><span class="sxs-lookup"><span data-stu-id="c0fb4-127">Response</span></span>

<span data-ttu-id="c0fb4-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c0fb4-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0fb4-130">示例</span><span class="sxs-lookup"><span data-stu-id="c0fb4-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0fb4-131">请求</span><span class="sxs-lookup"><span data-stu-id="c0fb4-131">Request</span></span>
<span data-ttu-id="c0fb4-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c0fb4-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c0fb4-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c0fb4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_oAuth2Permissiongrant"
}-->
```http
DELETE https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c0fb4-134">C#</span><span class="sxs-lookup"><span data-stu-id="c0fb4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c0fb4-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="c0fb4-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c0fb4-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="c0fb4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c0fb4-137">响应</span><span class="sxs-lookup"><span data-stu-id="c0fb4-137">Response</span></span>
<span data-ttu-id="c0fb4-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c0fb4-138">Here is an example of the response.</span></span> 
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
  "description": "Delete oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
