---
title: 删除 Outlook 类别
description: 删除指定的 outlookCategory 对象。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 1752d51d7463c575ab5957257132f27c72d78443
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33611561"
---
# <a name="delete-outlook-category"></a><span data-ttu-id="7ce8e-103">删除 Outlook 类别</span><span class="sxs-lookup"><span data-stu-id="7ce8e-103">Delete Outlook category</span></span>


<span data-ttu-id="7ce8e-104">删除指定的 [outlookCategory](../resources/outlookcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7ce8e-104">Delete the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ce8e-105">权限</span><span class="sxs-lookup"><span data-stu-id="7ce8e-105">Permissions</span></span>
<span data-ttu-id="7ce8e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7ce8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ce8e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7ce8e-108">Permission type</span></span>      | <span data-ttu-id="7ce8e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7ce8e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ce8e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7ce8e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7ce8e-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7ce8e-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="7ce8e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7ce8e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ce8e-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7ce8e-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="7ce8e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7ce8e-114">Application</span></span> | <span data-ttu-id="7ce8e-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7ce8e-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ce8e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7ce8e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7ce8e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="7ce8e-117">Request headers</span></span>
| <span data-ttu-id="7ce8e-118">名称</span><span class="sxs-lookup"><span data-stu-id="7ce8e-118">Name</span></span>      |<span data-ttu-id="7ce8e-119">说明</span><span class="sxs-lookup"><span data-stu-id="7ce8e-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7ce8e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ce8e-120">Authorization</span></span>  | <span data-ttu-id="7ce8e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7ce8e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ce8e-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="7ce8e-123">Request body</span></span>
<span data-ttu-id="7ce8e-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7ce8e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ce8e-125">响应</span><span class="sxs-lookup"><span data-stu-id="7ce8e-125">Response</span></span>

<span data-ttu-id="7ce8e-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7ce8e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ce8e-128">示例</span><span class="sxs-lookup"><span data-stu-id="7ce8e-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7ce8e-129">请求</span><span class="sxs-lookup"><span data-stu-id="7ce8e-129">Request</span></span>
<span data-ttu-id="7ce8e-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7ce8e-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["4b1c2495-54c9-4a5e-90a2-0ab0b31987d8"],
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/outlook/masterCategories/4b1c2495-54c9-4a5e-90a2-0ab0b31987d8
```
##### <a name="response"></a><span data-ttu-id="7ce8e-131">响应</span><span class="sxs-lookup"><span data-stu-id="7ce8e-131">Response</span></span>
<span data-ttu-id="7ce8e-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7ce8e-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "delete_outlookcategory",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7ce8e-133">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="7ce8e-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7ce8e-134">语言</span><span class="sxs-lookup"><span data-stu-id="7ce8e-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_outlookcategory-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7ce8e-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="7ce8e-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_outlookcategory-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/outlookcategory-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/outlookcategory-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
