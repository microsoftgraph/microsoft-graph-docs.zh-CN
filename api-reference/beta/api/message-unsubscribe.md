---
title: 消息： 取消订阅
description: 提交代表登录用户的电子邮件请求取消订阅电子邮件通讯组列表。 使用中的信息`List-Unsubscribe`标头。
ms.openlocfilehash: b4f72a0b629fb59074acbbd58f09a3c16118cc8c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045699"
---
# <a name="message-unsubscribe"></a><span data-ttu-id="8f3a3-104">消息： 取消订阅</span><span class="sxs-lookup"><span data-stu-id="8f3a3-104">message: unsubscribe</span></span>

> <span data-ttu-id="8f3a3-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8f3a3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f3a3-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8f3a3-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8f3a3-107">提交代表登录用户的电子邮件请求取消订阅电子邮件通讯组列表。</span><span class="sxs-lookup"><span data-stu-id="8f3a3-107">Submits a email request on behalf of the signed-in user to unsubscribe from an email distribution list.</span></span> <span data-ttu-id="8f3a3-108">使用中的信息`List-Unsubscribe`标头。</span><span class="sxs-lookup"><span data-stu-id="8f3a3-108">Uses the information in the `List-Unsubscribe` header.</span></span>

<span data-ttu-id="8f3a3-109">邮件发件人可以使用邮件列表以用户友好的方式通过包括一个选项以收件人退出。他们可以通过指定实现`List-Unsubscribe`关注[RFC 2369](https://www.faqs.org/rfcs/rfc2369.html)每个邮件中的页眉。</span><span class="sxs-lookup"><span data-stu-id="8f3a3-109">Message senders can use mailing lists in a user-friendly way by including an option for recipients to opt out. They can do so by specifying the `List-Unsubscribe` header in each message following [RFC-2369](https://www.faqs.org/rfcs/rfc2369.html).</span></span>

<span data-ttu-id="8f3a3-110">**注释**具体而言，以**取消**操作，发件人必须指定`mailto:`和不基于 URL 的取消信息。</span><span class="sxs-lookup"><span data-stu-id="8f3a3-110">**Note** In particular, for the **unsubscribe** action to work, the sender must specify `mailto:` and not URL-based unsubscribe information.</span></span>

<span data-ttu-id="8f3a3-111">设置该标题将对[邮件](../resources/message.md)实例与**unsubscribeEnabled**属性还设置`true`，并**unsubscribeData**属性设为标题数据。</span><span class="sxs-lookup"><span data-stu-id="8f3a3-111">Setting that header would also set the **unsubscribeEnabled** property of the [message](../resources/message.md) instance to `true`, and the **unsubscribeData** property to the header data.</span></span>

<span data-ttu-id="8f3a3-112">如果一条消息的**unsubscribeEnabled**属性是`true`，您可以使用**取消**操作取消类似今后的邮件用户管理邮件发件人。</span><span class="sxs-lookup"><span data-stu-id="8f3a3-112">If the **unsubscribeEnabled** property of a message is `true`, you can use the **unsubscribe** action to unsubscribe the user from similar future messages as managed by the message sender.</span></span>

<span data-ttu-id="8f3a3-113">成功，则**取消**操作会将邮件移到**已删除邮件**文件夹中。</span><span class="sxs-lookup"><span data-stu-id="8f3a3-113">A successful **unsubscribe** action moves the message to the **Deleted Items** folder.</span></span> <span data-ttu-id="8f3a3-114">发件人管理将来邮件通讯组从实际的用户的排除。</span><span class="sxs-lookup"><span data-stu-id="8f3a3-114">The actual exclusion of the user from future mail distribution is managed by the sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f3a3-115">权限</span><span class="sxs-lookup"><span data-stu-id="8f3a3-115">Permissions</span></span>
<span data-ttu-id="8f3a3-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8f3a3-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f3a3-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="8f3a3-118">Permission type</span></span>      | <span data-ttu-id="8f3a3-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8f3a3-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f3a3-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8f3a3-120">Delegated (work or school account)</span></span> | <span data-ttu-id="8f3a3-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="8f3a3-121">Mail.Send</span></span>    |
|<span data-ttu-id="8f3a3-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8f3a3-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f3a3-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="8f3a3-123">Mail.Send</span></span>    |
|<span data-ttu-id="8f3a3-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="8f3a3-124">Application</span></span> | <span data-ttu-id="8f3a3-125">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="8f3a3-125">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f3a3-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8f3a3-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/messages/{id}/unsubscribe
```
## <a name="request-headers"></a><span data-ttu-id="8f3a3-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="8f3a3-127">Request headers</span></span>
| <span data-ttu-id="8f3a3-128">名称</span><span class="sxs-lookup"><span data-stu-id="8f3a3-128">Name</span></span>       | <span data-ttu-id="8f3a3-129">类型</span><span class="sxs-lookup"><span data-stu-id="8f3a3-129">Type</span></span> | <span data-ttu-id="8f3a3-130">说明</span><span class="sxs-lookup"><span data-stu-id="8f3a3-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8f3a3-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f3a3-131">Authorization</span></span>  | <span data-ttu-id="8f3a3-132">string</span><span class="sxs-lookup"><span data-stu-id="8f3a3-132">string</span></span>  | <span data-ttu-id="8f3a3-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8f3a3-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f3a3-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="8f3a3-135">Request body</span></span>
<span data-ttu-id="8f3a3-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8f3a3-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f3a3-137">响应</span><span class="sxs-lookup"><span data-stu-id="8f3a3-137">Response</span></span>

<span data-ttu-id="8f3a3-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8f3a3-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f3a3-140">示例</span><span class="sxs-lookup"><span data-stu-id="8f3a3-140">Example</span></span>
<span data-ttu-id="8f3a3-141">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="8f3a3-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8f3a3-142">请求</span><span class="sxs-lookup"><span data-stu-id="8f3a3-142">Request</span></span>
<span data-ttu-id="8f3a3-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8f3a3-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_unsubscribe"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/{id}/unsubscribe
```

##### <a name="response"></a><span data-ttu-id="8f3a3-144">响应</span><span class="sxs-lookup"><span data-stu-id="8f3a3-144">Response</span></span>
<span data-ttu-id="8f3a3-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8f3a3-145">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: unsubscribe",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
