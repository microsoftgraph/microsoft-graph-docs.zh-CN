---
title: 删除 contactFolder
description: 删除默认 contactFolder 以外的 contactFolder。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 9ff9837b112f17c85edd2d382c46d9d8c1f22329
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33591440"
---
# <a name="delete-contactfolder"></a><span data-ttu-id="b0ed4-103">删除 contactFolder</span><span class="sxs-lookup"><span data-stu-id="b0ed4-103">Delete contactFolder</span></span>

<span data-ttu-id="b0ed4-104">删除默认 contactFolder 以外的 contactFolder。</span><span class="sxs-lookup"><span data-stu-id="b0ed4-104">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="b0ed4-105">权限</span><span class="sxs-lookup"><span data-stu-id="b0ed4-105">Permissions</span></span>
<span data-ttu-id="b0ed4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b0ed4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0ed4-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b0ed4-108">Permission type</span></span>      | <span data-ttu-id="b0ed4-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b0ed4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0ed4-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b0ed4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b0ed4-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0ed4-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="b0ed4-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b0ed4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0ed4-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0ed4-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="b0ed4-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b0ed4-114">Application</span></span> | <span data-ttu-id="b0ed4-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0ed4-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0ed4-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b0ed4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b0ed4-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="b0ed4-117">Request headers</span></span>
| <span data-ttu-id="b0ed4-118">名称</span><span class="sxs-lookup"><span data-stu-id="b0ed4-118">Name</span></span>       | <span data-ttu-id="b0ed4-119">类型</span><span class="sxs-lookup"><span data-stu-id="b0ed4-119">Type</span></span> | <span data-ttu-id="b0ed4-120">说明</span><span class="sxs-lookup"><span data-stu-id="b0ed4-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b0ed4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0ed4-121">Authorization</span></span>  | <span data-ttu-id="b0ed4-122">string</span><span class="sxs-lookup"><span data-stu-id="b0ed4-122">string</span></span>  | <span data-ttu-id="b0ed4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b0ed4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0ed4-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="b0ed4-125">Request body</span></span>
<span data-ttu-id="b0ed4-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b0ed4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0ed4-127">响应</span><span class="sxs-lookup"><span data-stu-id="b0ed4-127">Response</span></span>

<span data-ttu-id="b0ed4-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b0ed4-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0ed4-130">示例</span><span class="sxs-lookup"><span data-stu-id="b0ed4-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b0ed4-131">请求</span><span class="sxs-lookup"><span data-stu-id="b0ed4-131">Request</span></span>
<span data-ttu-id="b0ed4-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b0ed4-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="b0ed4-133">响应</span><span class="sxs-lookup"><span data-stu-id="b0ed4-133">Response</span></span>
<span data-ttu-id="b0ed4-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b0ed4-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b0ed4-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="b0ed4-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b0ed4-136">语言</span><span class="sxs-lookup"><span data-stu-id="b0ed4-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_contactfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b0ed4-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="b0ed4-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_contactfolder-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/contactfolder-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/contactfolder-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
