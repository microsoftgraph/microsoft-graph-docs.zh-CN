---
title: 删除应用程序
description: 删除应用程序。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e324afb6b0de7c6498796d1ccf4780e9db4eb15b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258511"
---
# <a name="delete-application"></a><span data-ttu-id="eecf9-103">删除应用程序</span><span class="sxs-lookup"><span data-stu-id="eecf9-103">Delete application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eecf9-104">删除应用程序。</span><span class="sxs-lookup"><span data-stu-id="eecf9-104">Deletes an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="eecf9-105">权限</span><span class="sxs-lookup"><span data-stu-id="eecf9-105">Permissions</span></span>
<span data-ttu-id="eecf9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eecf9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eecf9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="eecf9-108">Permission type</span></span>      | <span data-ttu-id="eecf9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eecf9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eecf9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eecf9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="eecf9-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="eecf9-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="eecf9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eecf9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eecf9-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="eecf9-113">Not supported.</span></span>    |
|<span data-ttu-id="eecf9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="eecf9-114">Application</span></span> | <span data-ttu-id="eecf9-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="eecf9-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eecf9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eecf9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="eecf9-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="eecf9-117">Request headers</span></span>
| <span data-ttu-id="eecf9-118">名称</span><span class="sxs-lookup"><span data-stu-id="eecf9-118">Name</span></span>       | <span data-ttu-id="eecf9-119">类型</span><span class="sxs-lookup"><span data-stu-id="eecf9-119">Type</span></span> | <span data-ttu-id="eecf9-120">说明</span><span class="sxs-lookup"><span data-stu-id="eecf9-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="eecf9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="eecf9-121">Authorization</span></span>  | <span data-ttu-id="eecf9-122">string</span><span class="sxs-lookup"><span data-stu-id="eecf9-122">string</span></span>  | <span data-ttu-id="eecf9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eecf9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eecf9-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="eecf9-125">Request body</span></span>
<span data-ttu-id="eecf9-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="eecf9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eecf9-127">响应</span><span class="sxs-lookup"><span data-stu-id="eecf9-127">Response</span></span>

<span data-ttu-id="eecf9-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="eecf9-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eecf9-130">示例</span><span class="sxs-lookup"><span data-stu-id="eecf9-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eecf9-131">请求</span><span class="sxs-lookup"><span data-stu-id="eecf9-131">Request</span></span>
<span data-ttu-id="eecf9-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eecf9-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_application"
}-->
```http
DELETE https://graph.microsoft.com/beta/applications/{id}
```
##### <a name="response"></a><span data-ttu-id="eecf9-133">响应</span><span class="sxs-lookup"><span data-stu-id="eecf9-133">Response</span></span>
<span data-ttu-id="eecf9-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="eecf9-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="eecf9-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="eecf9-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="eecf9-136">C#</span><span class="sxs-lookup"><span data-stu-id="eecf9-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_application-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eecf9-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="eecf9-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_application-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="eecf9-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="eecf9-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_application-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/application-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/application-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/application-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
