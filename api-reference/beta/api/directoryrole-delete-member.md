---
title: 删除目录角色成员
description: 从 directoryRole 中删除成员。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0921a946ce0b22a49a978530981184c06fbf84a3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260716"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="9f481-103">删除目录角色成员</span><span class="sxs-lookup"><span data-stu-id="9f481-103">Remove directory role member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f481-104">从 directoryRole 中删除成员。</span><span class="sxs-lookup"><span data-stu-id="9f481-104">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f481-105">权限</span><span class="sxs-lookup"><span data-stu-id="9f481-105">Permissions</span></span>

<span data-ttu-id="9f481-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9f481-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9f481-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9f481-108">Permission type</span></span>      | <span data-ttu-id="9f481-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9f481-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f481-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9f481-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9f481-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9f481-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9f481-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9f481-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f481-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f481-113">Not supported.</span></span>    |
|<span data-ttu-id="9f481-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9f481-114">Application</span></span> | <span data-ttu-id="9f481-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f481-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f481-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9f481-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryroles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="9f481-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="9f481-117">Request headers</span></span>

| <span data-ttu-id="9f481-118">名称</span><span class="sxs-lookup"><span data-stu-id="9f481-118">Name</span></span>       | <span data-ttu-id="9f481-119">类型</span><span class="sxs-lookup"><span data-stu-id="9f481-119">Type</span></span> | <span data-ttu-id="9f481-120">说明</span><span class="sxs-lookup"><span data-stu-id="9f481-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9f481-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f481-121">Authorization</span></span>  | <span data-ttu-id="9f481-122">string</span><span class="sxs-lookup"><span data-stu-id="9f481-122">string</span></span>  | <span data-ttu-id="9f481-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9f481-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f481-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9f481-125">Request body</span></span>

<span data-ttu-id="9f481-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9f481-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f481-127">响应</span><span class="sxs-lookup"><span data-stu-id="9f481-127">Response</span></span>

<span data-ttu-id="9f481-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9f481-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f481-130">示例</span><span class="sxs-lookup"><span data-stu-id="9f481-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9f481-131">请求</span><span class="sxs-lookup"><span data-stu-id="9f481-131">Request</span></span>

<span data-ttu-id="9f481-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9f481-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/beta/directoryroles/{id}/members/{id}/$ref
```

##### <a name="response"></a><span data-ttu-id="9f481-133">响应</span><span class="sxs-lookup"><span data-stu-id="9f481-133">Response</span></span>

<span data-ttu-id="9f481-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9f481-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9f481-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="9f481-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9f481-136">C#</span><span class="sxs-lookup"><span data-stu-id="9f481-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_directoryobject_from_directoryrole-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9f481-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="9f481-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_directoryobject_from_directoryrole-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="9f481-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="9f481-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_directoryobject_from_directoryrole-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete a member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryrole-delete-member.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/directoryrole-delete-member.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directoryrole-delete-member.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
