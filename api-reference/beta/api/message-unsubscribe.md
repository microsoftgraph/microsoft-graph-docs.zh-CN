---
title: '邮件: 取消订阅'
description: 代表已登录用户提交电子邮件请求, 以从电子邮件通讯组列表中取消订阅。 使用`List-Unsubscribe`标头中的信息。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 7e7723feb08c0e2d935781e0af7b5bd1098a4fc1
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266505"
---
# <a name="message-unsubscribe"></a><span data-ttu-id="ec50b-104">邮件: 取消订阅</span><span class="sxs-lookup"><span data-stu-id="ec50b-104">message: unsubscribe</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec50b-105">代表已登录用户提交电子邮件请求, 以从电子邮件通讯组列表中取消订阅。</span><span class="sxs-lookup"><span data-stu-id="ec50b-105">Submits a email request on behalf of the signed-in user to unsubscribe from an email distribution list.</span></span> <span data-ttu-id="ec50b-106">使用`List-Unsubscribe`标头中的信息。</span><span class="sxs-lookup"><span data-stu-id="ec50b-106">Uses the information in the `List-Unsubscribe` header.</span></span>

<span data-ttu-id="ec50b-107">邮件发件人可以通过包含一个用于选择收件人的选项, 以用户友好的方式使用邮寄列表。可以通过在[RFC-2369](https://www.faqs.org/rfcs/rfc2369.html)之后`List-Unsubscribe`的每封邮件中指定标头来执行此操作。</span><span class="sxs-lookup"><span data-stu-id="ec50b-107">Message senders can use mailing lists in a user-friendly way by including an option for recipients to opt out. They can do so by specifying the `List-Unsubscribe` header in each message following [RFC-2369](https://www.faqs.org/rfcs/rfc2369.html).</span></span>

<span data-ttu-id="ec50b-108">**注释**特别是, 要使**取消订阅**操作正常运行, 发件人`mailto:`必须指定而不是基于 URL 的取消订阅信息。</span><span class="sxs-lookup"><span data-stu-id="ec50b-108">**Note** In particular, for the **unsubscribe** action to work, the sender must specify `mailto:` and not URL-based unsubscribe information.</span></span>

<span data-ttu-id="ec50b-109">设置该标头也会将[消息](../resources/message.md)实例的**unsubscribeEnabled**属性设置为`true`, 并将**unsubscribeData**属性设置为标头数据。</span><span class="sxs-lookup"><span data-stu-id="ec50b-109">Setting that header would also set the **unsubscribeEnabled** property of the [message](../resources/message.md) instance to `true`, and the **unsubscribeData** property to the header data.</span></span>

<span data-ttu-id="ec50b-110">如果邮件的**unsubscribeEnabled**属性为`true`, 则可以使用 "**取消订阅**" 操作从邮件发件人托管的类似的未来邮件中取消订阅用户。</span><span class="sxs-lookup"><span data-stu-id="ec50b-110">If the **unsubscribeEnabled** property of a message is `true`, you can use the **unsubscribe** action to unsubscribe the user from similar future messages as managed by the message sender.</span></span>

<span data-ttu-id="ec50b-111">成功的**取消订阅**操作将邮件移动到 "**已删除邮件**" 文件夹。</span><span class="sxs-lookup"><span data-stu-id="ec50b-111">A successful **unsubscribe** action moves the message to the **Deleted Items** folder.</span></span> <span data-ttu-id="ec50b-112">用户从将来的邮件分发中实际排除的用户由发件人管理。</span><span class="sxs-lookup"><span data-stu-id="ec50b-112">The actual exclusion of the user from future mail distribution is managed by the sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec50b-113">权限</span><span class="sxs-lookup"><span data-stu-id="ec50b-113">Permissions</span></span>
<span data-ttu-id="ec50b-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ec50b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec50b-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec50b-116">Permission type</span></span>      | <span data-ttu-id="ec50b-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ec50b-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec50b-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec50b-118">Delegated (work or school account)</span></span> | <span data-ttu-id="ec50b-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ec50b-119">Mail.Send</span></span>    |
|<span data-ttu-id="ec50b-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec50b-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec50b-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ec50b-121">Mail.Send</span></span>    |
|<span data-ttu-id="ec50b-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec50b-122">Application</span></span> | <span data-ttu-id="ec50b-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ec50b-123">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec50b-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ec50b-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/messages/{id}/unsubscribe
```
## <a name="request-headers"></a><span data-ttu-id="ec50b-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="ec50b-125">Request headers</span></span>
| <span data-ttu-id="ec50b-126">名称</span><span class="sxs-lookup"><span data-stu-id="ec50b-126">Name</span></span>       | <span data-ttu-id="ec50b-127">类型</span><span class="sxs-lookup"><span data-stu-id="ec50b-127">Type</span></span> | <span data-ttu-id="ec50b-128">说明</span><span class="sxs-lookup"><span data-stu-id="ec50b-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ec50b-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec50b-129">Authorization</span></span>  | <span data-ttu-id="ec50b-130">string</span><span class="sxs-lookup"><span data-stu-id="ec50b-130">string</span></span>  | <span data-ttu-id="ec50b-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ec50b-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec50b-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="ec50b-133">Request body</span></span>
<span data-ttu-id="ec50b-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ec50b-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec50b-135">响应</span><span class="sxs-lookup"><span data-stu-id="ec50b-135">Response</span></span>

<span data-ttu-id="ec50b-p106">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ec50b-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec50b-138">示例</span><span class="sxs-lookup"><span data-stu-id="ec50b-138">Example</span></span>
<span data-ttu-id="ec50b-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="ec50b-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ec50b-140">请求</span><span class="sxs-lookup"><span data-stu-id="ec50b-140">Request</span></span>
<span data-ttu-id="ec50b-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ec50b-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_unsubscribe"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/{id}/unsubscribe
```

##### <a name="response"></a><span data-ttu-id="ec50b-142">响应</span><span class="sxs-lookup"><span data-stu-id="ec50b-142">Response</span></span>
<span data-ttu-id="ec50b-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ec50b-143">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ec50b-144">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="ec50b-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ec50b-145">C#</span><span class="sxs-lookup"><span data-stu-id="ec50b-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/message_unsubscribe-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ec50b-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="ec50b-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/message_unsubscribe-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ec50b-147">目标-C</span><span class="sxs-lookup"><span data-stu-id="ec50b-147">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/message_unsubscribe-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: unsubscribe",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-unsubscribe.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/message-unsubscribe.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/message-unsubscribe.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
