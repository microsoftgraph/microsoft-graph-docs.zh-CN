---
title: 删除目录设置
description: 删除目录设置。
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 0d1459e7ace8a2de6bae4fc696ac308cffca6392
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436692"
---
# <a name="delete-a-directory-setting"></a><span data-ttu-id="7d92a-103">删除目录设置</span><span class="sxs-lookup"><span data-stu-id="7d92a-103">Delete a directory setting</span></span>

<span data-ttu-id="7d92a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d92a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d92a-105">删除目录设置。</span><span class="sxs-lookup"><span data-stu-id="7d92a-105">Delete a directory setting.</span></span>

> <span data-ttu-id="7d92a-106">**注意**：此 API 的 /beta 版本仅适用于组。</span><span class="sxs-lookup"><span data-stu-id="7d92a-106">**Note**: The /beta version of this API only applies to groups.</span></span> <span data-ttu-id="7d92a-107">此 API 的 /v1.0 版本已重命名为 *Delete groupSettings。*</span><span class="sxs-lookup"><span data-stu-id="7d92a-107">The /v1.0 version of this API has been renamed to *Delete groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d92a-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="7d92a-108">Permissions</span></span>
<span data-ttu-id="7d92a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7d92a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d92a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7d92a-111">Permission type</span></span>      | <span data-ttu-id="7d92a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7d92a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d92a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7d92a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7d92a-114">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7d92a-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7d92a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7d92a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d92a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7d92a-116">Not supported.</span></span>    |
|<span data-ttu-id="7d92a-117">Application</span><span class="sxs-lookup"><span data-stu-id="7d92a-117">Application</span></span> | <span data-ttu-id="7d92a-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d92a-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d92a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7d92a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="7d92a-120">删除特定租户范围或组设置</span><span class="sxs-lookup"><span data-stu-id="7d92a-120">Delete a specific tenant-wide or group setting</span></span>
```http
DELETE /settings/{id}
DELETE /groups/{id}/settings/{id}

```
## <a name="request-headers"></a><span data-ttu-id="7d92a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="7d92a-121">Request headers</span></span>
| <span data-ttu-id="7d92a-122">名称</span><span class="sxs-lookup"><span data-stu-id="7d92a-122">Name</span></span>       | <span data-ttu-id="7d92a-123">说明</span><span class="sxs-lookup"><span data-stu-id="7d92a-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7d92a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d92a-124">Authorization</span></span>  | <span data-ttu-id="7d92a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7d92a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d92a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7d92a-127">Request body</span></span>
<span data-ttu-id="7d92a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7d92a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d92a-129">响应</span><span class="sxs-lookup"><span data-stu-id="7d92a-129">Response</span></span>

<span data-ttu-id="7d92a-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7d92a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d92a-132">示例</span><span class="sxs-lookup"><span data-stu-id="7d92a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7d92a-133">请求</span><span class="sxs-lookup"><span data-stu-id="7d92a-133">Request</span></span>
<span data-ttu-id="7d92a-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7d92a-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7d92a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="7d92a-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directorysetting"
}-->
```http
DELETE https://graph.microsoft.com/beta/settings/{id}
```
# <a name="c"></a>[<span data-ttu-id="7d92a-136">C#</span><span class="sxs-lookup"><span data-stu-id="7d92a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directorysetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7d92a-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7d92a-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directorysetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7d92a-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7d92a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directorysetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7d92a-139">Java</span><span class="sxs-lookup"><span data-stu-id="7d92a-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directorysetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7d92a-140">响应</span><span class="sxs-lookup"><span data-stu-id="7d92a-140">Response</span></span>
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
  "description": "Delete directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


