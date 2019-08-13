---
title: 删除 oAuth2PermissionGrant
description: 删除 oAuth2PermissionGrant。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 280e33b9e970b72d569cb92dfc5e6f478bf1ceab
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342668"
---
# <a name="delete-oauth2permissiongrant"></a><span data-ttu-id="f1318-103">删除 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="f1318-103">Delete oAuth2PermissionGrant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1318-104">删除 oAuth2PermissionGrant。</span><span class="sxs-lookup"><span data-stu-id="f1318-104">Delete an oAuth2PermissionGrant.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1318-105">权限</span><span class="sxs-lookup"><span data-stu-id="f1318-105">Permissions</span></span>
<span data-ttu-id="f1318-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f1318-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f1318-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f1318-108">Permission type</span></span>      | <span data-ttu-id="f1318-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f1318-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1318-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f1318-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f1318-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f1318-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f1318-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f1318-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1318-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1318-113">Not supported.</span></span>    |
|<span data-ttu-id="f1318-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f1318-114">Application</span></span> | <span data-ttu-id="f1318-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1318-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1318-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f1318-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /oAuth2Permissiongrants/{id}
DELETE /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
DELETE /drive/root/createdByUser/oAuth2Permissiongrants/{id}

```
## <a name="request-headers"></a><span data-ttu-id="f1318-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="f1318-117">Request headers</span></span>
| <span data-ttu-id="f1318-118">名称</span><span class="sxs-lookup"><span data-stu-id="f1318-118">Name</span></span>       | <span data-ttu-id="f1318-119">类型</span><span class="sxs-lookup"><span data-stu-id="f1318-119">Type</span></span> | <span data-ttu-id="f1318-120">说明</span><span class="sxs-lookup"><span data-stu-id="f1318-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f1318-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1318-121">Authorization</span></span>  | <span data-ttu-id="f1318-122">string</span><span class="sxs-lookup"><span data-stu-id="f1318-122">string</span></span>  | <span data-ttu-id="f1318-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f1318-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1318-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f1318-125">Request body</span></span>
<span data-ttu-id="f1318-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f1318-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1318-127">响应</span><span class="sxs-lookup"><span data-stu-id="f1318-127">Response</span></span>

<span data-ttu-id="f1318-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f1318-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1318-130">示例</span><span class="sxs-lookup"><span data-stu-id="f1318-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1318-131">请求</span><span class="sxs-lookup"><span data-stu-id="f1318-131">Request</span></span>
<span data-ttu-id="f1318-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f1318-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f1318-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f1318-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_oAuth2Permissiongrant"
}-->
```http
DELETE https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f1318-134">C#</span><span class="sxs-lookup"><span data-stu-id="f1318-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f1318-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1318-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f1318-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="f1318-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f1318-137">Java</span><span class="sxs-lookup"><span data-stu-id="f1318-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-oauth2permissiongrant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f1318-138">响应</span><span class="sxs-lookup"><span data-stu-id="f1318-138">Response</span></span>
<span data-ttu-id="f1318-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f1318-139">Here is an example of the response.</span></span> 
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
