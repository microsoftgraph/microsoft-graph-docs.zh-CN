---
title: 删除 contactFolder
description: 删除默认 contactFolder 以外的 contactFolder。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 192a5679449728c3dea6e46376427b3c47d5d229
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261297"
---
# <a name="delete-contactfolder"></a><span data-ttu-id="7c7fc-103">删除 contactFolder</span><span class="sxs-lookup"><span data-stu-id="7c7fc-103">Delete contactFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c7fc-104">删除默认 contactFolder 以外的 contactFolder。</span><span class="sxs-lookup"><span data-stu-id="7c7fc-104">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="7c7fc-105">权限</span><span class="sxs-lookup"><span data-stu-id="7c7fc-105">Permissions</span></span>
<span data-ttu-id="7c7fc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7c7fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c7fc-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7c7fc-108">Permission type</span></span>      | <span data-ttu-id="7c7fc-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7c7fc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c7fc-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7c7fc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7c7fc-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c7fc-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="7c7fc-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7c7fc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c7fc-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c7fc-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="7c7fc-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7c7fc-114">Application</span></span> | <span data-ttu-id="7c7fc-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c7fc-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c7fc-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7c7fc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7c7fc-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="7c7fc-117">Request headers</span></span>
| <span data-ttu-id="7c7fc-118">名称</span><span class="sxs-lookup"><span data-stu-id="7c7fc-118">Name</span></span>       | <span data-ttu-id="7c7fc-119">类型</span><span class="sxs-lookup"><span data-stu-id="7c7fc-119">Type</span></span> | <span data-ttu-id="7c7fc-120">说明</span><span class="sxs-lookup"><span data-stu-id="7c7fc-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7c7fc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c7fc-121">Authorization</span></span>  | <span data-ttu-id="7c7fc-122">string</span><span class="sxs-lookup"><span data-stu-id="7c7fc-122">string</span></span>  | <span data-ttu-id="7c7fc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7c7fc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c7fc-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="7c7fc-125">Request body</span></span>
<span data-ttu-id="7c7fc-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7c7fc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c7fc-127">响应</span><span class="sxs-lookup"><span data-stu-id="7c7fc-127">Response</span></span>

<span data-ttu-id="7c7fc-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7c7fc-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c7fc-130">示例</span><span class="sxs-lookup"><span data-stu-id="7c7fc-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7c7fc-131">请求</span><span class="sxs-lookup"><span data-stu-id="7c7fc-131">Request</span></span>
<span data-ttu-id="7c7fc-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7c7fc-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="7c7fc-133">响应</span><span class="sxs-lookup"><span data-stu-id="7c7fc-133">Response</span></span>
<span data-ttu-id="7c7fc-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7c7fc-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7c7fc-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="7c7fc-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7c7fc-136">C#</span><span class="sxs-lookup"><span data-stu-id="7c7fc-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_contactfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7c7fc-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="7c7fc-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_contactfolder-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7c7fc-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="7c7fc-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_contactfolder-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/contactfolder-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/contactfolder-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/contactfolder-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
