---
title: 'message: createReplyAll'
description: 创建草稿以回复指定邮件的发件人和所有收件人。 然后，可以更新草稿，将回复内容添加到**正文**，或更改其他邮件属性，或者仅发送草稿。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 65b8180050f074844bdda504ddcccc4360a264c4
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33612763"
---
# <a name="message-createreplyall"></a><span data-ttu-id="47460-104">message: createReplyAll</span><span class="sxs-lookup"><span data-stu-id="47460-104">message: createReplyAll</span></span>

<span data-ttu-id="47460-105">创建草稿以回复指定[邮件](../resources/message.md)的发件人和所有收件人。</span><span class="sxs-lookup"><span data-stu-id="47460-105">Create a draft to reply to the sender and all the recipients of the specified [message](../resources/message.md).</span></span> <span data-ttu-id="47460-106">然后，可以[更新](../api/message-update.md)草稿，将回复内容添加到**正文**，或更改其他邮件属性，或者仅[发送](../api/message-send.md)草稿。</span><span class="sxs-lookup"><span data-stu-id="47460-106">You can then [update](../api/message-update.md) the draft to add reply content to the **body** or change other message properties, or, simply [send](../api/message-send.md) the draft.</span></span>

## <a name="permissions"></a><span data-ttu-id="47460-107">权限</span><span class="sxs-lookup"><span data-stu-id="47460-107">Permissions</span></span>
<span data-ttu-id="47460-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="47460-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47460-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="47460-110">Permission type</span></span>      | <span data-ttu-id="47460-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="47460-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47460-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="47460-112">Delegated (work or school account)</span></span> | <span data-ttu-id="47460-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47460-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="47460-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="47460-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47460-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47460-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="47460-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="47460-116">Application</span></span> | <span data-ttu-id="47460-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47460-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="47460-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="47460-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/messages/{id}/createReplyAll
POST /me/mailFolders/{id}/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReplyAll
```
## <a name="request-headers"></a><span data-ttu-id="47460-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="47460-119">Request headers</span></span>
| <span data-ttu-id="47460-120">名称</span><span class="sxs-lookup"><span data-stu-id="47460-120">Name</span></span>       | <span data-ttu-id="47460-121">类型</span><span class="sxs-lookup"><span data-stu-id="47460-121">Type</span></span> | <span data-ttu-id="47460-122">说明</span><span class="sxs-lookup"><span data-stu-id="47460-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="47460-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="47460-123">Authorization</span></span>  | <span data-ttu-id="47460-124">string</span><span class="sxs-lookup"><span data-stu-id="47460-124">string</span></span>  | <span data-ttu-id="47460-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="47460-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="47460-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="47460-127">Request body</span></span>
<span data-ttu-id="47460-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="47460-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47460-129">响应</span><span class="sxs-lookup"><span data-stu-id="47460-129">Response</span></span>

<span data-ttu-id="47460-130">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="47460-130">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47460-131">示例</span><span class="sxs-lookup"><span data-stu-id="47460-131">Example</span></span>
<span data-ttu-id="47460-132">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="47460-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="47460-133">请求</span><span class="sxs-lookup"><span data-stu-id="47460-133">Request</span></span>
<span data-ttu-id="47460-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="47460-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createreplyall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createReplyAll
```

##### <a name="response"></a><span data-ttu-id="47460-135">响应</span><span class="sxs-lookup"><span data-stu-id="47460-135">Response</span></span>
<span data-ttu-id="47460-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="47460-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="47460-139">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="47460-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="47460-140">语言</span><span class="sxs-lookup"><span data-stu-id="47460-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/message_createreplyall-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="47460-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="47460-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/message_createreplyall-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: createReplyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/message-createreplyall.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/message-createreplyall.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
