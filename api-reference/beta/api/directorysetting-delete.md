---
title: 删除目录设置
description: 删除目录设置。
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9bb979df437f9f3a18ad1fbc5351c39e041ae5b0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43375784"
---
# <a name="delete-a-directory-setting"></a><span data-ttu-id="79265-103">删除目录设置</span><span class="sxs-lookup"><span data-stu-id="79265-103">Delete a directory setting</span></span>

<span data-ttu-id="79265-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79265-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79265-105">删除目录设置。</span><span class="sxs-lookup"><span data-stu-id="79265-105">Delete a directory setting.</span></span>

> <span data-ttu-id="79265-106">**注意**：此 API 的/beta 版本仅适用于组。</span><span class="sxs-lookup"><span data-stu-id="79265-106">**Note**: The /beta version of this API only applies to groups.</span></span> <span data-ttu-id="79265-107">此 API 的/v1.0 版本已重命名为*删除 groupSettings*。</span><span class="sxs-lookup"><span data-stu-id="79265-107">The /v1.0 version of this API has been renamed to *Delete groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="79265-108">权限</span><span class="sxs-lookup"><span data-stu-id="79265-108">Permissions</span></span>
<span data-ttu-id="79265-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="79265-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79265-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="79265-111">Permission type</span></span>      | <span data-ttu-id="79265-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="79265-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79265-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79265-113">Delegated (work or school account)</span></span> | <span data-ttu-id="79265-114">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="79265-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="79265-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79265-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79265-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="79265-116">Not supported.</span></span>    |
|<span data-ttu-id="79265-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="79265-117">Application</span></span> | <span data-ttu-id="79265-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79265-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="79265-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="79265-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="79265-120">删除特定的租户范围或组设置</span><span class="sxs-lookup"><span data-stu-id="79265-120">Delete a specific tenant-wide or group setting</span></span>
```http
DELETE /settings/{id}
DELETE /groups/{id}/settings/{id}

```
## <a name="request-headers"></a><span data-ttu-id="79265-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="79265-121">Request headers</span></span>
| <span data-ttu-id="79265-122">名称</span><span class="sxs-lookup"><span data-stu-id="79265-122">Name</span></span>       | <span data-ttu-id="79265-123">说明</span><span class="sxs-lookup"><span data-stu-id="79265-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="79265-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="79265-124">Authorization</span></span>  | <span data-ttu-id="79265-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="79265-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="79265-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="79265-127">Request body</span></span>
<span data-ttu-id="79265-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="79265-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79265-129">响应</span><span class="sxs-lookup"><span data-stu-id="79265-129">Response</span></span>

<span data-ttu-id="79265-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="79265-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79265-132">示例</span><span class="sxs-lookup"><span data-stu-id="79265-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="79265-133">请求</span><span class="sxs-lookup"><span data-stu-id="79265-133">Request</span></span>
<span data-ttu-id="79265-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="79265-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="79265-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="79265-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directorysetting"
}-->
```http
DELETE https://graph.microsoft.com/beta/settings/{id}
```
# <a name="c"></a>[<span data-ttu-id="79265-136">C#</span><span class="sxs-lookup"><span data-stu-id="79265-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directorysetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79265-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79265-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directorysetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79265-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79265-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directorysetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="79265-139">响应</span><span class="sxs-lookup"><span data-stu-id="79265-139">Response</span></span>
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
