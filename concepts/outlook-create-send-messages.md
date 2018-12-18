---
title: 自动创建、发送和处理邮件
description: 电子邮件通过 Microsoft Graph 中的邮件资源表示。
author: angelgolfer-ms
ms.openlocfilehash: fa549395ad55f0eb2d2d16748250fda1745d8b92
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332527"
---
# <a name="automate-creating-sending-and-processing-messages"></a><span data-ttu-id="2f8f7-103">自动创建、发送和处理邮件</span><span class="sxs-lookup"><span data-stu-id="2f8f7-103">Automate creating, sending, and processing messages</span></span>

<span data-ttu-id="2f8f7-104">电子邮件通过 Microsoft Graph 中的[邮件](/graph/api/resources/message?view=graph-rest-1.0)资源表示。</span><span class="sxs-lookup"><span data-stu-id="2f8f7-104">Emails are represented by the [message](/graph/api/resources/message?view=graph-rest-1.0) resource in Microsoft Graph.</span></span>

<span data-ttu-id="2f8f7-105">默认情况下，邮件由 **ID** 属性中的唯一条目 ID 标识。</span><span class="sxs-lookup"><span data-stu-id="2f8f7-105">By default, messages are identified by a unique entry ID in the **id** property.</span></span> <span data-ttu-id="2f8f7-106">当最初创建、保存为草稿或发送邮件时，存储提供程序会为邮件分配一个条目 ID。</span><span class="sxs-lookup"><span data-stu-id="2f8f7-106">When a message is initially created and saved as a draft or sent, the store provider assigns the message an entry ID.</span></span> <span data-ttu-id="2f8f7-107">默认情况下，当将邮件复制或移动到另一个文件夹、存储空间或 .PST 文件时，该 ID 会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2f8f7-107">By default, that ID changes when the message is copied or moved to another folder, store, or .PST file.</span></span> <span data-ttu-id="2f8f7-108">可以通过当前 ID 引用邮件，以便后续处理。</span><span class="sxs-lookup"><span data-stu-id="2f8f7-108">You reference the message by its current ID for further processing.</span></span>

## <a name="creating-and-sending-mail"></a><span data-ttu-id="2f8f7-109">创建和发送邮件</span><span class="sxs-lookup"><span data-stu-id="2f8f7-109">Creating and sending mail</span></span>

<span data-ttu-id="2f8f7-110">在 Outlook 中，你可以在同一 [sendMail](/graph/api/user-sendmail?view=graph-rest-1.0) 操作中创建和发送电子邮件，或者可以[创建](/graph/api/user-post-messages?view=graph-rest-1.0)草稿，然后[添加内容](/graph/api/message-update?view=graph-rest-1.0)并[发送](/graph/api/message-send?view=graph-rest-1.0)此草稿。</span><span class="sxs-lookup"><span data-stu-id="2f8f7-110">In Outlook, you can create and send an email in the same [sendMail](/graph/api/user-sendmail?view=graph-rest-1.0) action, or you can [create](/graph/api/user-post-messages?view=graph-rest-1.0) a draft, subsequently [add content](/graph/api/message-update?view=graph-rest-1.0) and [send](/graph/api/message-send?view=graph-rest-1.0) the draft.</span></span>

<span data-ttu-id="2f8f7-111">同样，在回复电子邮件时，也可以使用相同的操作（[答复](/graph/api/message-reply?view=graph-rest-1.0)、[全部答复](/graph/api/message-replyall?view=graph-rest-1.0)或[转发](/graph/api/message-forward?view=graph-rest-1.0)）创建和发送响应。</span><span class="sxs-lookup"><span data-stu-id="2f8f7-111">Similarly, when responding to an email, you can create and send the response in the same action ([reply](/graph/api/message-reply?view=graph-rest-1.0), [reply-all](/graph/api/message-replyall?view=graph-rest-1.0), or [forward](/graph/api/message-forward?view=graph-rest-1.0)).</span></span> <span data-ttu-id="2f8f7-112">或者，你可以为响应（[答复](/graph/api/message-createreply?view=graph-rest-1.0)、[全部答复](/graph/api/message-createreplyall?view=graph-rest-1.0)或[转发](/graph/api/message-createforward?view=graph-rest-1.0)）创建草稿，[添加内容](/graph/api/message-update?view=graph-rest-1.0)），然后稍后[发送](/graph/api/message-send?view=graph-rest-1.0)此草稿。</span><span class="sxs-lookup"><span data-stu-id="2f8f7-112">Or, you can create a draft for the response ([reply](/graph/api/message-createreply?view=graph-rest-1.0), [reply-all](/graph/api/message-createreplyall?view=graph-rest-1.0), or [forward](/graph/api/message-createforward?view=graph-rest-1.0)), [add content](/graph/api/message-update?view=graph-rest-1.0), and then [send](/graph/api/message-send?view=graph-rest-1.0) the draft at a later time.</span></span>

<span data-ttu-id="2f8f7-113">要以编程方式区分草稿和已发送邮件，请选中 **isDraft** 属性。</span><span class="sxs-lookup"><span data-stu-id="2f8f7-113">To distinguish between a draft and a sent message programmatically, check the **isDraft** property.</span></span>

<span data-ttu-id="2f8f7-114">默认情况下，草稿邮件保存在 `Drafts` 文件夹中，已发送邮件保存在 `Sent Items` 文件夹中。</span><span class="sxs-lookup"><span data-stu-id="2f8f7-114">By default, draft messages are saved in the `Drafts` folder, sent messages are saved in the `Sent Items` folder.</span></span> <span data-ttu-id="2f8f7-115">为方便起见，可以通过相应的[已知文件夹名称](/graph/api/resources/mailfolder?view=graph-rest-1.0)来识别 Drafts 文件夹和 SentItems 文件夹。</span><span class="sxs-lookup"><span data-stu-id="2f8f7-115">For convenience, you can identify the Drafts folder and SentItems folder by their corresponding [well-known folder names](/graph/api/resources/mailfolder?view=graph-rest-1.0).</span></span> 

### <a name="setting-the-from-and-sender-properties"></a><span data-ttu-id="2f8f7-116">设置 from 和 sender 属性</span><span class="sxs-lookup"><span data-stu-id="2f8f7-116">Setting the from and sender properties</span></span>

<span data-ttu-id="2f8f7-117">撰写邮件时，Outlook 在大多数情况下会将 **from** 和 **sender** 属性设置为同一登录用户。</span><span class="sxs-lookup"><span data-stu-id="2f8f7-117">When a message is being composed, in most cases, Outlook sets the **from** and **sender** properties to the same signed-in user.</span></span> <span data-ttu-id="2f8f7-118">你可以在以下情况下更新这些属性：</span><span class="sxs-lookup"><span data-stu-id="2f8f7-118">You can update these properties in the following scenarios:</span></span>

- <span data-ttu-id="2f8f7-p105">如果 Exchange 管理员已将邮箱的 **sendAs** 权限分配给其他一些用户，可以更改 **from** 属性。为此，管理员可以在 Azure 门户中选择邮箱所有者的**邮箱权限**，也可以使用 Exchange 管理中心或 Windows PowerShell Add-ADPermission cmdlet。然后，可以编程方式将 **from** 属性设置为，对相应邮箱拥有 **sendAs** 权限的用户之一。</span><span class="sxs-lookup"><span data-stu-id="2f8f7-p105">The **from** property can be changed if the Exchange administrator has assigned **sendAs** rights of the mailbox to some other users. The administrator can do this by selecting **Mailbox Permissions** of the mailbox owner in the Azure portal, or by using the Exchange Admin Center or a Windows PowerShell Add-ADPermission cmdlet. Then, you can programmatically set the **from** property to one of these users who have **sendAs** rights for that mailbox.</span></span>
- <span data-ttu-id="2f8f7-122">如果邮箱所有者已委派一个或多个用户能够从该邮箱发送邮件，则可以更改 **sender** 属性。</span><span class="sxs-lookup"><span data-stu-id="2f8f7-122">The **sender** property can be changed if the mailbox owner has delegated one or more users to be able to send messages from that mailbox.</span></span> <span data-ttu-id="2f8f7-123">可以在 Outlook 中委派邮箱所有者。</span><span class="sxs-lookup"><span data-stu-id="2f8f7-123">The mailbox owner can delegate in Outlook.</span></span> <span data-ttu-id="2f8f7-124">当代理代表邮箱所有者发送邮件时，Outlook 将 **sender** 属性设置为代理的帐户，**from** 属性仍保持为邮箱所有者。</span><span class="sxs-lookup"><span data-stu-id="2f8f7-124">When a delegate sends a message on behalf of the mailbox owner, Outlook sets the **sender** property to the delegate’s account, and the **from** property remains as the mailbox owner.</span></span> <span data-ttu-id="2f8f7-125">通过编程方式，你可以将 **sender** 属性设置为已拥有邮箱委派权限的用户。</span><span class="sxs-lookup"><span data-stu-id="2f8f7-125">Programmatically, you can set the **sender** property to a user who has got delegate permissions for that mailbox.</span></span>

## <a name="using-mailtips-to-check-recipient-status-and-save-time-preview"></a><span data-ttu-id="2f8f7-126">使用邮件提醒检查收件人状态并节省时间（预览版）</span><span class="sxs-lookup"><span data-stu-id="2f8f7-126">Using MailTips to check recipient status and save time (preview)</span></span>

<span data-ttu-id="2f8f7-127">在发送电子邮件之前，可使用[邮件提醒](/graph/api/resources/mailtips?view=graph-rest-beta)做出明智的决定。</span><span class="sxs-lookup"><span data-stu-id="2f8f7-127">Use [MailTips](/graph/api/resources/mailtips?view=graph-rest-beta) to make smart decisions before sending an email.</span></span>
<span data-ttu-id="2f8f7-128">邮件提醒可以告诉你诸如收件人的邮箱限于特定发件人，或者需要批准才能向收件人发送电子邮件等信息。</span><span class="sxs-lookup"><span data-stu-id="2f8f7-128">MailTips can tell you information such as the recipient's mailbox is restricted to specific senders, or approval is required for emailing the recipient.</span></span>


## <a name="reading-messages-with-control-over-the-body-format-returned"></a><span data-ttu-id="2f8f7-129">阅读邮件并控制返回的正文格式</span><span class="sxs-lookup"><span data-stu-id="2f8f7-129">Reading messages with control over the body format returned</span></span>

<span data-ttu-id="2f8f7-130">可以通过引用邮件 ID 来[阅读邮箱中的邮件](/graph/api/message-get?view=graph-rest-1.0)：</span><span class="sxs-lookup"><span data-stu-id="2f8f7-130">You can [read a message](/graph/api/message-get?view=graph-rest-1.0) in a mailbox by referencing its ID:</span></span>

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AAMkADhMGAAA="]
}-->
```http
GET /me/messages/AAMkADhMGAAA=
```

或者，也可以[获取特定文件夹中的邮件](/graph/api/user-list-messages?view=graph-rest-1.0)。 <span data-ttu-id="2f8f7-132">例如，阅读单点登录用户的“草稿”文件夹中的邮件：</span><span class="sxs-lookup"><span data-stu-id="2f8f7-132">For example, to read messages in the signed-in user's Drafts folder:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailfolders('Drafts')
```

<span data-ttu-id="2f8f7-133">Outlook 邮件正文可以是 HTML 或文本，其中 HTML 作为 GET 响应中返回的默认邮件正文类型。</span><span class="sxs-lookup"><span data-stu-id="2f8f7-133">The body of an Outlook message can be either HTML or text, with HTML as the default message body type returned in a GET response.</span></span>

<span data-ttu-id="2f8f7-134">获取邮件时，你可以指定以下请求标头以文本格式返回 **body** 和 **uniqueBody** 属性：</span><span class="sxs-lookup"><span data-stu-id="2f8f7-134">When getting a message, you can specify the following request header to return the **body** and **uniqueBody** properties in text format:</span></span>

```http
Prefer: outlook.body-content-type="text"
```

<span data-ttu-id="2f8f7-135">你可以指定以下标头（或直接跳过标头），以 HTML 格式获取邮件正文：</span><span class="sxs-lookup"><span data-stu-id="2f8f7-135">You can specify the following header, or, just skip the header, to get the message body in HTML format:</span></span>

```http
Prefer: outlook.body-content-type="html"
```

<span data-ttu-id="2f8f7-136">当指定任一标头时，成功的响应将包含相应的 `Preference-Applied` 标头：</span><span class="sxs-lookup"><span data-stu-id="2f8f7-136">When you specify either header, a successful response would include the corresponding `Preference-Applied` header:</span></span>

- <span data-ttu-id="2f8f7-137">对于文本格式请求：`Preference-Applied: outlook.body-content-type="text"`</span><span class="sxs-lookup"><span data-stu-id="2f8f7-137">For text format requests: `Preference-Applied: outlook.body-content-type="text"`</span></span>
- <span data-ttu-id="2f8f7-138">对于 HTML 格式请求：`Preference-Applied: outlook.body-content-type="html"`</span><span class="sxs-lookup"><span data-stu-id="2f8f7-138">For HTML format requests: `Preference-Applied: outlook.body-content-type="html"`</span></span>

<span data-ttu-id="2f8f7-139">默认情况下，如果正文是 HTML 格式，那么在 REST 响应中返回正文内容之前，Outlook 将删除嵌入 **body** 属性中的任何具有潜在不安全性的 HTML（例如 JavaScript）。</span><span class="sxs-lookup"><span data-stu-id="2f8f7-139">If the body is HTML, by default, Outlook removes any potentially unsafe HTML (for example, JavaScript) embedded in the **body** property before returning the body content in a REST response.</span></span>

<span data-ttu-id="2f8f7-140">若要获取整个原始 HTML 内容，请包括以下 HTTP 请求标头：</span><span class="sxs-lookup"><span data-stu-id="2f8f7-140">To get the entire, original HTML content, include the following HTTP request header:</span></span>

```http
Prefer: outlook.allow-unsafe-html
```

## <a name="integrating-with--social-gesture-preview"></a><span data-ttu-id="2f8f7-141">与“@”社交手势集成（预览版）</span><span class="sxs-lookup"><span data-stu-id="2f8f7-141">Integrating with '@' social gesture (preview)</span></span>

<span data-ttu-id="2f8f7-142">@-mention 是提醒用户邮件中是否有提到他们的通知。</span><span class="sxs-lookup"><span data-stu-id="2f8f7-142">@-mentions are notifications to alert users if they are mentioned in messages.</span></span> <span data-ttu-id="2f8f7-143">[mention](/graph/api/resources/mention?view=graph-rest-beta)资源使应用能够在电子邮件中设置和获取常见的在线社交手势，即“@”前缀。</span><span class="sxs-lookup"><span data-stu-id="2f8f7-143">The [mention](/graph/api/resources/mention?view=graph-rest-beta) resource enables apps to set and get the common online social gesture, the '@' prefix, in emails.</span></span>
<span data-ttu-id="2f8f7-144">可以执行下列操作：</span><span class="sxs-lookup"><span data-stu-id="2f8f7-144">You can:</span></span>

- <span data-ttu-id="2f8f7-145">在[创建邮件](/graph/api/user-post-messages?view=graph-rest-beta#request-2)时创建 @-mention</span><span class="sxs-lookup"><span data-stu-id="2f8f7-145">Create @-mentions when [creating a message](/graph/api/user-post-messages?view=graph-rest-beta#request-2)</span></span>
- [<span data-ttu-id="2f8f7-146">获取用户邮箱中包含用户 @-mention 的所有邮件</span><span class="sxs-lookup"><span data-stu-id="2f8f7-146">Get all the messages in a user's mailbox that contain an @-mention of the user</span></span>](/graph/api/user-list-messages?view=graph-rest-beta#request-2)
- [<span data-ttu-id="2f8f7-147">获取所有 @-mention 就形成一封邮件</span><span class="sxs-lookup"><span data-stu-id="2f8f7-147">Get all the @-mention is a message</span></span>](/graph/api/message-get?view=graph-rest-beta#request-2)

## <a name="other-shared-capabilities"></a><span data-ttu-id="2f8f7-148">其他共享的功能</span><span class="sxs-lookup"><span data-stu-id="2f8f7-148">Other shared capabilities</span></span>

<span data-ttu-id="2f8f7-149">利用以下在 Microsoft Graph 实体之间共享的常用功能：</span><span class="sxs-lookup"><span data-stu-id="2f8f7-149">Take advantage of the following common capabilities that are shared among Microsoft Graph entities:</span></span>

- <span data-ttu-id="2f8f7-150">发生一种或多种类型的更改时（如创建或更新邮件），订阅邮件的[更改通知](/graph/api/resources/webhooks?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="2f8f7-150">Subscribe to [change notifications](/graph/api/resources/webhooks?view=graph-rest-1.0) on messages when one or more types of changes occur, such as message creation or update.</span></span>
- <span data-ttu-id="2f8f7-151">[跟踪文件夹中邮件的这些增量更改](delta-query-messages.md)</span><span class="sxs-lookup"><span data-stu-id="2f8f7-151">[Track these incremental changes to messages in a folder](delta-query-messages.md).</span></span>
- <span data-ttu-id="2f8f7-152">创建[开放扩展](extensibility-overview.md#open-extensions)或[架构扩展](extensibility-overview.md#schema-extensions)，以将自定义数据添加到邮件实例。</span><span class="sxs-lookup"><span data-stu-id="2f8f7-152">Create [open extensions](extensibility-overview.md#open-extensions) or [schema extensions](extensibility-overview.md#schema-extensions) to add custom data to a message instance.</span></span>
- <span data-ttu-id="2f8f7-153">当 Outlook MAPI 属性尚未通过 Microsoft Graph API 元数据公开时，在邮件实例中创建[扩展属性](/graph/api/resources/extended-properties-overview?view=graph-rest-1.0)以存储这些属性的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="2f8f7-153">Create [extended properties](/graph/api/resources/extended-properties-overview?view=graph-rest-1.0) in a message instance to store custom data for Outlook MAPI properties, when these properties are not already exposed in the Microsoft Graph API metadata.</span></span>

## <a name="next-steps"></a><span data-ttu-id="2f8f7-154">后续步骤</span><span class="sxs-lookup"><span data-stu-id="2f8f7-154">Next steps</span></span>

<span data-ttu-id="2f8f7-155">详细了解以下信息：</span><span class="sxs-lookup"><span data-stu-id="2f8f7-155">Find out more about:</span></span>

- [<span data-ttu-id="2f8f7-156">为什么与 Outlook 邮件集成</span><span class="sxs-lookup"><span data-stu-id="2f8f7-156">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- [<span data-ttu-id="2f8f7-157">获取 Outlook 资源的不可变标识符（预览版）</span><span class="sxs-lookup"><span data-stu-id="2f8f7-157">Get immutable identifiers for Outlook resources (preview)</span></span>](outlook-immutable-id.md)
- <span data-ttu-id="2f8f7-158">[使用邮件 API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) 及其在 Microsoft Graph v1.0 中的[用例](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases)。</span><span class="sxs-lookup"><span data-stu-id="2f8f7-158">[Using the mail API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) and its [use cases](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) in Microsoft Graph v1.0.</span></span>
