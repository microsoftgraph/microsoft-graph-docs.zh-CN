---
title: 删除应用程序
description: 删除应用程序。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f40359f7c4b0cdbffdb22b6a8a7236a3ba0038c6
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636287"
---
# <a name="delete-application"></a><span data-ttu-id="55cd3-103">删除应用程序</span><span class="sxs-lookup"><span data-stu-id="55cd3-103">Delete application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55cd3-104">删除应用程序。</span><span class="sxs-lookup"><span data-stu-id="55cd3-104">Deletes an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="55cd3-105">权限</span><span class="sxs-lookup"><span data-stu-id="55cd3-105">Permissions</span></span>
<span data-ttu-id="55cd3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="55cd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55cd3-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="55cd3-108">Permission type</span></span>      | <span data-ttu-id="55cd3-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="55cd3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55cd3-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="55cd3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="55cd3-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="55cd3-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="55cd3-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="55cd3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55cd3-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="55cd3-113">Not supported.</span></span>    |
|<span data-ttu-id="55cd3-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="55cd3-114">Application</span></span> | <span data-ttu-id="55cd3-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="55cd3-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="55cd3-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="55cd3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="55cd3-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="55cd3-117">Request headers</span></span>
| <span data-ttu-id="55cd3-118">名称</span><span class="sxs-lookup"><span data-stu-id="55cd3-118">Name</span></span>       | <span data-ttu-id="55cd3-119">类型</span><span class="sxs-lookup"><span data-stu-id="55cd3-119">Type</span></span> | <span data-ttu-id="55cd3-120">说明</span><span class="sxs-lookup"><span data-stu-id="55cd3-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="55cd3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="55cd3-121">Authorization</span></span>  | <span data-ttu-id="55cd3-122">string</span><span class="sxs-lookup"><span data-stu-id="55cd3-122">string</span></span>  | <span data-ttu-id="55cd3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="55cd3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55cd3-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="55cd3-125">Request body</span></span>
<span data-ttu-id="55cd3-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="55cd3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55cd3-127">响应</span><span class="sxs-lookup"><span data-stu-id="55cd3-127">Response</span></span>

<span data-ttu-id="55cd3-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="55cd3-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55cd3-130">示例</span><span class="sxs-lookup"><span data-stu-id="55cd3-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="55cd3-131">请求</span><span class="sxs-lookup"><span data-stu-id="55cd3-131">Request</span></span>
<span data-ttu-id="55cd3-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="55cd3-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_application"
}-->
```http
DELETE https://graph.microsoft.com/beta/applications/{id}
```
##### <a name="response"></a><span data-ttu-id="55cd3-133">响应</span><span class="sxs-lookup"><span data-stu-id="55cd3-133">Response</span></span>
<span data-ttu-id="55cd3-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="55cd3-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="55cd3-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="55cd3-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="55cd3-136">语言</span><span class="sxs-lookup"><span data-stu-id="55cd3-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_application-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="55cd3-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="55cd3-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_application-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/application-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/application-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
