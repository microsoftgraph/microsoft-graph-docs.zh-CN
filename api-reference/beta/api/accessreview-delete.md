---
title: 删除 accessReview
description: 在 Azure AD 访问评审功能中，删除 accessReview 对象。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 8877c0778f9924995c75dd47b331608d4994a62f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048503"
---
# <a name="delete-accessreview"></a><span data-ttu-id="3c4a9-103">删除 accessReview</span><span class="sxs-lookup"><span data-stu-id="3c4a9-103">Delete accessReview</span></span>

<span data-ttu-id="3c4a9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c4a9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c4a9-105">在 Azure AD [访问评审](../resources/accessreviews-root.md) 功能中，删除 [accessReview](../resources/accessreview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3c4a9-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3c4a9-106">权限</span><span class="sxs-lookup"><span data-stu-id="3c4a9-106">Permissions</span></span>
<span data-ttu-id="3c4a9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3c4a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c4a9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c4a9-109">Permission type</span></span>                        | <span data-ttu-id="3c4a9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3c4a9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c4a9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c4a9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3c4a9-112">AccessReview.ReadWrite.Membership、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c4a9-112">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="3c4a9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c4a9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c4a9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c4a9-114">Not supported.</span></span> |
|<span data-ttu-id="3c4a9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c4a9-115">Application</span></span>                            | <span data-ttu-id="3c4a9-116">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="3c4a9-116">AccessReview.ReadWrite.Membership</span></span> |

<span data-ttu-id="3c4a9-117">调用方还应具有 ProgramControl.ReadWrite.All 权限，以便它可以删除 [programControl](../resources/programcontrol.md)。</span><span class="sxs-lookup"><span data-stu-id="3c4a9-117">The caller should also have ProgramControl.ReadWrite.All permission, so that it can delete a [programControl](../resources/programcontrol.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="3c4a9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c4a9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews/{reviewId}
```
## <a name="request-headers"></a><span data-ttu-id="3c4a9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c4a9-119">Request headers</span></span>
| <span data-ttu-id="3c4a9-120">名称</span><span class="sxs-lookup"><span data-stu-id="3c4a9-120">Name</span></span>         | <span data-ttu-id="3c4a9-121">类型</span><span class="sxs-lookup"><span data-stu-id="3c4a9-121">Type</span></span>        | <span data-ttu-id="3c4a9-122">说明</span><span class="sxs-lookup"><span data-stu-id="3c4a9-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3c4a9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c4a9-123">Authorization</span></span> | <span data-ttu-id="3c4a9-124">string</span><span class="sxs-lookup"><span data-stu-id="3c4a9-124">string</span></span> | <span data-ttu-id="3c4a9-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="3c4a9-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c4a9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c4a9-127">Request body</span></span>
<span data-ttu-id="3c4a9-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3c4a9-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="3c4a9-129">响应</span><span class="sxs-lookup"><span data-stu-id="3c4a9-129">Response</span></span>
<span data-ttu-id="3c4a9-p103">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3c4a9-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c4a9-132">示例</span><span class="sxs-lookup"><span data-stu-id="3c4a9-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3c4a9-133">请求</span><span class="sxs-lookup"><span data-stu-id="3c4a9-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3c4a9-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c4a9-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accessReview"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/
```
# <a name="c"></a>[<span data-ttu-id="3c4a9-135">C#</span><span class="sxs-lookup"><span data-stu-id="3c4a9-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c4a9-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c4a9-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c4a9-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c4a9-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3c4a9-138">Java</span><span class="sxs-lookup"><span data-stu-id="3c4a9-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3c4a9-139">响应</span><span class="sxs-lookup"><span data-stu-id="3c4a9-139">Response</span></span>
><span data-ttu-id="3c4a9-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3c4a9-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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


