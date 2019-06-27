---
title: 删除 accessReview
description: 在 "Azure AD access 评论" 功能中, 删除 accessReview 对象。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d7a7434d4de008ce2a3f597636c30fcf014f3de8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258980"
---
# <a name="delete-accessreview"></a><span data-ttu-id="88345-103">删除 accessReview</span><span class="sxs-lookup"><span data-stu-id="88345-103">Delete accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88345-104">在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中, 删除[accessReview](../resources/accessreview.md)对象。</span><span class="sxs-lookup"><span data-stu-id="88345-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="88345-105">权限</span><span class="sxs-lookup"><span data-stu-id="88345-105">Permissions</span></span>
<span data-ttu-id="88345-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88345-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88345-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="88345-108">Permission type</span></span>                        | <span data-ttu-id="88345-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="88345-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="88345-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88345-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="88345-111">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88345-111">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="88345-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88345-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88345-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="88345-113">Not supported.</span></span> |
|<span data-ttu-id="88345-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="88345-114">Application</span></span>                            | <span data-ttu-id="88345-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="88345-115">Not supported.</span></span> |

<span data-ttu-id="88345-116">调用方还应具有 ProgramControl 权限, 以便它可以删除[ProgramControl](../resources/programcontrol.md)。</span><span class="sxs-lookup"><span data-stu-id="88345-116">The caller should also have ProgramControl.ReadWrite.All permission, so that it can delete a [programControl](../resources/programcontrol.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="88345-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88345-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="88345-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="88345-118">Request headers</span></span>
| <span data-ttu-id="88345-119">名称</span><span class="sxs-lookup"><span data-stu-id="88345-119">Name</span></span>         | <span data-ttu-id="88345-120">类型</span><span class="sxs-lookup"><span data-stu-id="88345-120">Type</span></span>        | <span data-ttu-id="88345-121">说明</span><span class="sxs-lookup"><span data-stu-id="88345-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="88345-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="88345-122">Authorization</span></span> | <span data-ttu-id="88345-123">string</span><span class="sxs-lookup"><span data-stu-id="88345-123">string</span></span> | <span data-ttu-id="88345-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="88345-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="88345-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="88345-126">Request body</span></span>
<span data-ttu-id="88345-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="88345-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="88345-128">响应</span><span class="sxs-lookup"><span data-stu-id="88345-128">Response</span></span>
<span data-ttu-id="88345-p103">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="88345-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88345-131">示例</span><span class="sxs-lookup"><span data-stu-id="88345-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="88345-132">请求</span><span class="sxs-lookup"><span data-stu-id="88345-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_accessReview"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/
```
##### <a name="response"></a><span data-ttu-id="88345-133">响应</span><span class="sxs-lookup"><span data-stu-id="88345-133">Response</span></span>
><span data-ttu-id="88345-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="88345-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="88345-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="88345-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="88345-137">C#</span><span class="sxs-lookup"><span data-stu-id="88345-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_accessReview-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="88345-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="88345-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_accessReview-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="88345-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="88345-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_accessReview-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/accessreview-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
