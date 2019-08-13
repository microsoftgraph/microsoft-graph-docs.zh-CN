---
title: 删除 accessReview
description: 在 "Azure AD access 评论" 功能中, 删除 accessReview 对象。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4ded5c3776dbc66a6433482a40fb95ec248c2f95
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36316118"
---
# <a name="delete-accessreview"></a><span data-ttu-id="bdafd-103">删除 accessReview</span><span class="sxs-lookup"><span data-stu-id="bdafd-103">Delete accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdafd-104">在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中, 删除[accessReview](../resources/accessreview.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bdafd-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bdafd-105">权限</span><span class="sxs-lookup"><span data-stu-id="bdafd-105">Permissions</span></span>
<span data-ttu-id="bdafd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bdafd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdafd-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="bdafd-108">Permission type</span></span>                        | <span data-ttu-id="bdafd-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bdafd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="bdafd-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bdafd-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bdafd-111">AccessReview、AccessReview 和所有</span><span class="sxs-lookup"><span data-stu-id="bdafd-111">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="bdafd-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bdafd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdafd-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="bdafd-113">Not supported.</span></span> |
|<span data-ttu-id="bdafd-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="bdafd-114">Application</span></span>                            | <span data-ttu-id="bdafd-115">AccessReview 的成员资格</span><span class="sxs-lookup"><span data-stu-id="bdafd-115">AccessReview.ReadWrite.Membership</span></span> |

<span data-ttu-id="bdafd-116">调用方还应具有 ProgramControl 权限, 以便它可以删除[ProgramControl](../resources/programcontrol.md)。</span><span class="sxs-lookup"><span data-stu-id="bdafd-116">The caller should also have ProgramControl.ReadWrite.All permission, so that it can delete a [programControl](../resources/programcontrol.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="bdafd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bdafd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="bdafd-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bdafd-118">Request headers</span></span>
| <span data-ttu-id="bdafd-119">名称</span><span class="sxs-lookup"><span data-stu-id="bdafd-119">Name</span></span>         | <span data-ttu-id="bdafd-120">类型</span><span class="sxs-lookup"><span data-stu-id="bdafd-120">Type</span></span>        | <span data-ttu-id="bdafd-121">说明</span><span class="sxs-lookup"><span data-stu-id="bdafd-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="bdafd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdafd-122">Authorization</span></span> | <span data-ttu-id="bdafd-123">string</span><span class="sxs-lookup"><span data-stu-id="bdafd-123">string</span></span> | <span data-ttu-id="bdafd-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="bdafd-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bdafd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bdafd-126">Request body</span></span>
<span data-ttu-id="bdafd-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bdafd-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="bdafd-128">响应</span><span class="sxs-lookup"><span data-stu-id="bdafd-128">Response</span></span>
<span data-ttu-id="bdafd-p103">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="bdafd-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdafd-131">示例</span><span class="sxs-lookup"><span data-stu-id="bdafd-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bdafd-132">请求</span><span class="sxs-lookup"><span data-stu-id="bdafd-132">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bdafd-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="bdafd-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accessReview"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bdafd-134">C#</span><span class="sxs-lookup"><span data-stu-id="bdafd-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bdafd-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bdafd-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bdafd-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="bdafd-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bdafd-137">Java</span><span class="sxs-lookup"><span data-stu-id="bdafd-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bdafd-138">响应</span><span class="sxs-lookup"><span data-stu-id="bdafd-138">Response</span></span>
><span data-ttu-id="bdafd-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bdafd-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

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
  ]
}
-->
