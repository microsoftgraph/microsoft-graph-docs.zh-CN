---
title: SendReminder accessReview
description: '在 Azure AD 访问评审功能中，向当前处于活动状态的 accessReview 的审阅者发送提醒。  目标对象可以是一次性访问评审，也可以作为定期访问评审的实例。 '
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 6176f1c0762df35682f61077ee88028d80a5613e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439267"
---
# <a name="sendreminder-accessreview"></a><span data-ttu-id="af577-104">SendReminder accessReview</span><span class="sxs-lookup"><span data-stu-id="af577-104">SendReminder accessReview</span></span>

<span data-ttu-id="af577-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af577-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af577-106">在 Azure AD [访问评审](../resources/accessreviews-root.md) 功能中，向当前处于活动状态 [的 accessReview](../resources/accessreview.md)的审阅者发送提醒。</span><span class="sxs-lookup"><span data-stu-id="af577-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, send a reminder to the reviewers of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="af577-107">目标对象可以是一次性访问评审，也可以作为定期访问评审的实例。</span><span class="sxs-lookup"><span data-stu-id="af577-107">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span> 

## <a name="permissions"></a><span data-ttu-id="af577-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="af577-108">Permissions</span></span>
<span data-ttu-id="af577-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="af577-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af577-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="af577-111">Permission type</span></span>                        | <span data-ttu-id="af577-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="af577-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="af577-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="af577-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="af577-114">AccessReview.ReadWrite.Membership、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af577-114">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="af577-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="af577-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af577-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="af577-116">Not supported.</span></span> |
|<span data-ttu-id="af577-117">Application</span><span class="sxs-lookup"><span data-stu-id="af577-117">Application</span></span>                            | <span data-ttu-id="af577-118">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="af577-118">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="af577-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="af577-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/sendReminder
```
## <a name="request-headers"></a><span data-ttu-id="af577-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="af577-120">Request headers</span></span>
| <span data-ttu-id="af577-121">名称</span><span class="sxs-lookup"><span data-stu-id="af577-121">Name</span></span>         | <span data-ttu-id="af577-122">类型</span><span class="sxs-lookup"><span data-stu-id="af577-122">Type</span></span>        | <span data-ttu-id="af577-123">说明</span><span class="sxs-lookup"><span data-stu-id="af577-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="af577-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="af577-124">Authorization</span></span> | <span data-ttu-id="af577-125">string</span><span class="sxs-lookup"><span data-stu-id="af577-125">string</span></span> | <span data-ttu-id="af577-p104">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="af577-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="af577-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="af577-128">Request body</span></span>
<span data-ttu-id="af577-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="af577-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="af577-130">响应</span><span class="sxs-lookup"><span data-stu-id="af577-130">Response</span></span>
<span data-ttu-id="af577-p105">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="af577-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af577-133">示例</span><span class="sxs-lookup"><span data-stu-id="af577-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="af577-134">请求</span><span class="sxs-lookup"><span data-stu-id="af577-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="af577-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="af577-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/sendReminder
```
# <a name="c"></a>[<span data-ttu-id="af577-136">C#</span><span class="sxs-lookup"><span data-stu-id="af577-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/sendreminder-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="af577-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="af577-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/sendreminder-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="af577-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="af577-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/sendreminder-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="af577-139">Java</span><span class="sxs-lookup"><span data-stu-id="af577-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/sendreminder-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="af577-140">响应</span><span class="sxs-lookup"><span data-stu-id="af577-140">Response</span></span>
><span data-ttu-id="af577-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="af577-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "SendReminder accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


