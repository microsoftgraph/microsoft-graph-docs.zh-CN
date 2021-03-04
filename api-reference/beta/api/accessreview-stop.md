---
title: Stop accessReview
description: 在 Azure AD 访问评审功能中，停止当前处于活动状态的 accessReview。  目标对象可以是一次性访问评审，也可以作为定期访问评审的实例。   (若要阻止定期访问评审启动将来实例，请更新它以更改其计划的结束日期) 。  访问评审停止后，审阅者将不再提供输入，并且可以应用访问评审决策。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: d2ff44fe7f0c4fd21af0373edd72e4c3f6097491
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439268"
---
# <a name="stop-accessreview"></a><span data-ttu-id="6094c-106">Stop accessReview</span><span class="sxs-lookup"><span data-stu-id="6094c-106">Stop accessReview</span></span>

<span data-ttu-id="6094c-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6094c-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6094c-108">在 Azure AD[访问评审](../resources/accessreviews-root.md)功能中，停止当前处于活动状态[的 accessReview。](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="6094c-108">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, stop a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="6094c-109">目标对象可以是一次性访问评审，也可以作为定期访问评审的实例。</span><span class="sxs-lookup"><span data-stu-id="6094c-109">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="6094c-110"> (若要阻止定期访问评审启动将来实例，请更新它以更改其计划的[](accessreview-update.md)结束日期) 。</span><span class="sxs-lookup"><span data-stu-id="6094c-110">(To prevent a recurring access review from starting future instances, [update it](accessreview-update.md) to change its scheduled end date).</span></span>  <span data-ttu-id="6094c-111">访问评审停止后，审阅者将不再提供输入，并且可以应用访问评审决策。</span><span class="sxs-lookup"><span data-stu-id="6094c-111">After the access review stops, reviewers can no longer give input, and the access review decisions can be applied.</span></span>
## <a name="permissions"></a><span data-ttu-id="6094c-112">Permissions</span><span class="sxs-lookup"><span data-stu-id="6094c-112">Permissions</span></span>
<span data-ttu-id="6094c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6094c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6094c-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="6094c-115">Permission type</span></span>                        | <span data-ttu-id="6094c-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6094c-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6094c-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6094c-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="6094c-118">AccessReview.ReadWrite.Membership、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6094c-118">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="6094c-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6094c-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6094c-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="6094c-120">Not supported.</span></span> |
|<span data-ttu-id="6094c-121">Application</span><span class="sxs-lookup"><span data-stu-id="6094c-121">Application</span></span>                            | <span data-ttu-id="6094c-122">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="6094c-122">AccessReview.ReadWrite.Membership</span></span>  |

## <a name="http-request"></a><span data-ttu-id="6094c-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6094c-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/stop
```
## <a name="request-headers"></a><span data-ttu-id="6094c-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="6094c-124">Request headers</span></span>
| <span data-ttu-id="6094c-125">名称</span><span class="sxs-lookup"><span data-stu-id="6094c-125">Name</span></span>         | <span data-ttu-id="6094c-126">类型</span><span class="sxs-lookup"><span data-stu-id="6094c-126">Type</span></span>        | <span data-ttu-id="6094c-127">说明</span><span class="sxs-lookup"><span data-stu-id="6094c-127">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="6094c-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="6094c-128">Authorization</span></span> | <span data-ttu-id="6094c-129">string</span><span class="sxs-lookup"><span data-stu-id="6094c-129">string</span></span> | <span data-ttu-id="6094c-p104">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="6094c-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6094c-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="6094c-132">Request body</span></span>
<span data-ttu-id="6094c-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6094c-133">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="6094c-134">响应</span><span class="sxs-lookup"><span data-stu-id="6094c-134">Response</span></span>
<span data-ttu-id="6094c-p105">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6094c-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6094c-137">示例</span><span class="sxs-lookup"><span data-stu-id="6094c-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6094c-138">请求</span><span class="sxs-lookup"><span data-stu-id="6094c-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6094c-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="6094c-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "stop_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/stop
```
# <a name="c"></a>[<span data-ttu-id="6094c-140">C#</span><span class="sxs-lookup"><span data-stu-id="6094c-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/stop-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6094c-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6094c-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/stop-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6094c-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6094c-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/stop-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6094c-143">Java</span><span class="sxs-lookup"><span data-stu-id="6094c-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/stop-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6094c-144">响应</span><span class="sxs-lookup"><span data-stu-id="6094c-144">Response</span></span>
><span data-ttu-id="6094c-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6094c-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Stop accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


