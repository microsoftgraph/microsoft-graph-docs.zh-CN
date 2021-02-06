---
title: message： unsubscribe
description: 代表登录用户提交电子邮件请求以取消订阅电子邮件通讯组列表。 使用标头 `List-Unsubscribe` 中的信息。
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7bf800fe385c75c6d472f9cee40f55ec81633640
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131094"
---
# <a name="message-unsubscribe"></a><span data-ttu-id="b39e8-104">message： unsubscribe</span><span class="sxs-lookup"><span data-stu-id="b39e8-104">message: unsubscribe</span></span>

<span data-ttu-id="b39e8-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b39e8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b39e8-106">代表登录用户提交电子邮件请求以取消订阅电子邮件通讯组列表。</span><span class="sxs-lookup"><span data-stu-id="b39e8-106">Submits a email request on behalf of the signed-in user to unsubscribe from an email distribution list.</span></span> <span data-ttu-id="b39e8-107">使用标头 `List-Unsubscribe` 中的信息。</span><span class="sxs-lookup"><span data-stu-id="b39e8-107">Uses the information in the `List-Unsubscribe` header.</span></span>

<span data-ttu-id="b39e8-108">邮件发件人可以通过包括收件人选择退出的选项，以用户友好的方式使用邮件列表。他们可以通过在 `List-Unsubscribe` [RFC-2369](https://www.faqs.org/rfcs/rfc2369.html)之后的每封邮件中指定邮件头来这样做。</span><span class="sxs-lookup"><span data-stu-id="b39e8-108">Message senders can use mailing lists in a user-friendly way by including an option for recipients to opt out. They can do so by specifying the `List-Unsubscribe` header in each message following [RFC-2369](https://www.faqs.org/rfcs/rfc2369.html).</span></span>

<span data-ttu-id="b39e8-109">**注意** 具体而言，若要使 **取消** 订阅操作正常工作，发件人必须指定基于 `mailto:` URL 的取消订阅信息，而不是基于 URL 的取消订阅信息。</span><span class="sxs-lookup"><span data-stu-id="b39e8-109">**Note** In particular, for the **unsubscribe** action to work, the sender must specify `mailto:` and not URL-based unsubscribe information.</span></span>

<span data-ttu-id="b39e8-110">设置该标头还会将邮件实例 **的 unsubscribeEnabled** [](../resources/message.md)属性设置为 `true` ，将 **unsubscribeData** 属性设置为邮件头数据。</span><span class="sxs-lookup"><span data-stu-id="b39e8-110">Setting that header would also set the **unsubscribeEnabled** property of the [message](../resources/message.md) instance to `true`, and the **unsubscribeData** property to the header data.</span></span>

<span data-ttu-id="b39e8-111">如果 **邮件的 unsubscribeEnabled** 属性是，您可以使用取消订阅操作取消订阅用户与邮件发件人管理的类似未来 `true` 邮件。 </span><span class="sxs-lookup"><span data-stu-id="b39e8-111">If the **unsubscribeEnabled** property of a message is `true`, you can use the **unsubscribe** action to unsubscribe the user from similar future messages as managed by the message sender.</span></span>

<span data-ttu-id="b39e8-112">成功的 **取消订阅** 操作会将邮件移动到 **"已删除邮件"** 文件夹。</span><span class="sxs-lookup"><span data-stu-id="b39e8-112">A successful **unsubscribe** action moves the message to the **Deleted Items** folder.</span></span> <span data-ttu-id="b39e8-113">用户在将来的邮件分发中的实际排除情况由发件人管理。</span><span class="sxs-lookup"><span data-stu-id="b39e8-113">The actual exclusion of the user from future mail distribution is managed by the sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="b39e8-114">权限</span><span class="sxs-lookup"><span data-stu-id="b39e8-114">Permissions</span></span>
<span data-ttu-id="b39e8-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b39e8-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b39e8-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="b39e8-117">Permission type</span></span>      | <span data-ttu-id="b39e8-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b39e8-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b39e8-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b39e8-119">Delegated (work or school account)</span></span> | <span data-ttu-id="b39e8-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="b39e8-120">Mail.Send</span></span>    |
|<span data-ttu-id="b39e8-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b39e8-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b39e8-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="b39e8-122">Mail.Send</span></span>    |
|<span data-ttu-id="b39e8-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="b39e8-123">Application</span></span> | <span data-ttu-id="b39e8-124">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="b39e8-124">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="b39e8-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b39e8-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/messages/{id}/unsubscribe
```
## <a name="request-headers"></a><span data-ttu-id="b39e8-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="b39e8-126">Request headers</span></span>
| <span data-ttu-id="b39e8-127">名称</span><span class="sxs-lookup"><span data-stu-id="b39e8-127">Name</span></span>       | <span data-ttu-id="b39e8-128">类型</span><span class="sxs-lookup"><span data-stu-id="b39e8-128">Type</span></span> | <span data-ttu-id="b39e8-129">说明</span><span class="sxs-lookup"><span data-stu-id="b39e8-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b39e8-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="b39e8-130">Authorization</span></span>  | <span data-ttu-id="b39e8-131">string</span><span class="sxs-lookup"><span data-stu-id="b39e8-131">string</span></span>  | <span data-ttu-id="b39e8-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b39e8-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b39e8-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="b39e8-134">Request body</span></span>
<span data-ttu-id="b39e8-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b39e8-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b39e8-136">响应</span><span class="sxs-lookup"><span data-stu-id="b39e8-136">Response</span></span>

<span data-ttu-id="b39e8-p106">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b39e8-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b39e8-139">示例</span><span class="sxs-lookup"><span data-stu-id="b39e8-139">Example</span></span>
<span data-ttu-id="b39e8-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="b39e8-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b39e8-141">请求</span><span class="sxs-lookup"><span data-stu-id="b39e8-141">Request</span></span>
<span data-ttu-id="b39e8-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b39e8-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b39e8-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="b39e8-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_unsubscribe"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/{id}/unsubscribe
```
# <a name="c"></a>[<span data-ttu-id="b39e8-144">C#</span><span class="sxs-lookup"><span data-stu-id="b39e8-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-unsubscribe-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b39e8-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b39e8-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-unsubscribe-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b39e8-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b39e8-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-unsubscribe-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b39e8-147">Java</span><span class="sxs-lookup"><span data-stu-id="b39e8-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-unsubscribe-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b39e8-148">响应</span><span class="sxs-lookup"><span data-stu-id="b39e8-148">Response</span></span>
<span data-ttu-id="b39e8-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b39e8-149">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

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
  ]
}
-->


