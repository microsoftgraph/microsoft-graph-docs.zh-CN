# <a name="create-and-send-outlook-messages"></a><span data-ttu-id="c57e3-101">创建和发送 Outlook 邮件</span><span class="sxs-lookup"><span data-stu-id="c57e3-101">Create and send Outlook messages</span></span>

<span data-ttu-id="c57e3-102">电子邮件通过 Microsoft Graph 中的[邮件](../api-reference/v1.0/resources/message.md)资源表示。</span><span class="sxs-lookup"><span data-stu-id="c57e3-102">Emails are represented by the [message](../api-reference/v1.0/resources/message.md) resource in Microsoft Graph.</span></span>

<span data-ttu-id="c57e3-103">默认情况下，邮件由 **ID** 属性中的唯一条目 ID 标识。</span><span class="sxs-lookup"><span data-stu-id="c57e3-103">By default, messages are identified by a unique entry ID in the **id** property.</span></span> <span data-ttu-id="c57e3-104">当邮件最初保存为草稿或已发送时，存储提供程序会为消息分配一个条目 ID。</span><span class="sxs-lookup"><span data-stu-id="c57e3-104">A store provider assigns a message an entry ID when the message is initially saved as a draft or sent.</span></span> <span data-ttu-id="c57e3-105">当将邮件复制或移动到另一个文件夹、存储或 .PST 文件时，该 ID 会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c57e3-105">That ID changes when the message is copied or moved to another folder, store, or .PST file.</span></span>

## <a name="creating-and-sending-mail"></a><span data-ttu-id="c57e3-106">创建和发送邮件</span><span class="sxs-lookup"><span data-stu-id="c57e3-106">Creating and sending mail</span></span>

<span data-ttu-id="c57e3-107">在 Outlook 中，你可以在同一 [sendMail](../api-reference/v1.0/api/user_sendmail.md) 操作中创建和发送电子邮件，或者可以[创建](../api-reference/v1.0/api/user_post_messages.md)草稿，然后[添加内容](../api-reference/v1.0/api/message_update.md)并[发送](../api-reference/v1.0/api/message_send.md)此草稿。</span><span class="sxs-lookup"><span data-stu-id="c57e3-107">In Outlook, you can create and send an email in the same [sendMail](../api-reference/v1.0/api/user_sendmail.md) action, or you can [create](../api-reference/v1.0/api/user_post_messages.md) a draft, subsequently [add content](../api-reference/v1.0/api/message_update.md) and [send](../api-reference/v1.0/api/message_send.md) the draft.</span></span>

<span data-ttu-id="c57e3-108">同样，在回复电子邮件时，也可以使用相同的操作（[答复](../api-reference/v1.0/api/message_reply.md)、[全部答复](../api-reference/v1.0/api//message_replyall.md)或[转发](../api-reference/v1.0/api/message_forward.md)）创建和发送响应。</span><span class="sxs-lookup"><span data-stu-id="c57e3-108">Similarly, when responding to an email, you can create and send the response in the same action ([reply](../api-reference/v1.0/api/message_reply.md), [reply-all](../api-reference/v1.0/api//message_replyall.md), or [forward](../api-reference/v1.0/api/message_forward.md)).</span></span> <span data-ttu-id="c57e3-109">或者，你可以为响应（[答复](../api-reference/v1.0/api/message_createreply.md)、[全部答复](../api-reference/v1.0/api//message_createreplyall.md)或[转发](../api-reference/v1.0/api/message_createforward.md)）创建草稿，[添加内容](../api-reference/v1.0/api/message_update.md)），然后稍后[发送](../api-reference/v1.0/api/message_send.md)此草稿。</span><span class="sxs-lookup"><span data-stu-id="c57e3-109">Or, you can create a draft for the response ([reply](../api-reference/v1.0/api/message_createreply.md), [reply-all](../api-reference/v1.0/api//message_createreplyall.md), or [forward](../api-reference/v1.0/api/message_createforward.md)), [add content](../api-reference/v1.0/api/message_update.md), and then [send](../api-reference/v1.0/api/message_send.md) the draft at a later time.</span></span>

<span data-ttu-id="c57e3-110">要以编程方式区分草稿和已发送邮件，请选中 **isDraft** 属性。</span><span class="sxs-lookup"><span data-stu-id="c57e3-110">To distinguish between a draft and a sent message programmatically, check the **isDraft** property.</span></span>

<span data-ttu-id="c57e3-111">默认情况下，草稿邮件保存在 `Drafts` 文件夹中，已发送邮件保存在 `Sent Items` 文件夹中。</span><span class="sxs-lookup"><span data-stu-id="c57e3-111">By default, draft messages are saved in the `Drafts` folder, sent messages are saved in the `Sent Items` folder.</span></span> <span data-ttu-id="c57e3-112">为方便起见，可以通过相应的[已知文件夹名称](../api-reference/v1.0/resources/mailfolder.md)来识别 Drafts 文件夹和 SentItems 文件夹。</span><span class="sxs-lookup"><span data-stu-id="c57e3-112">For convenience, you can identify the Drafts folder and SentItems folder by their corresponding [well-known folder names](../api-reference/v1.0/resources/mailfolder.md).</span></span> <span data-ttu-id="c57e3-113">例如，可以执行以下操作[获取 Drafts 文件夹中的邮件](../api-reference/v1.0/api/user_list_messages.md)：</span><span class="sxs-lookup"><span data-stu-id="c57e3-113">For example, you can do the following to [get the messages](../api-reference/v1.0/api/user_list_messages.md) in the Drafts folder:</span></span>

```http
GET /me/mailfolders('Drafts')
```

### <a name="body-format-and-malicious-script"></a><span data-ttu-id="c57e3-114">正文格式和恶意脚本</span><span class="sxs-lookup"><span data-stu-id="c57e3-114">Body format and malicious script</span></span>

<!-- Remove the following 2 sections from the message.md topics
-->

<span data-ttu-id="c57e3-115">邮件正文可以是 HTML 或文本，其中 HTML 作为 GET 响应中返回的默认邮件正文类型。</span><span class="sxs-lookup"><span data-stu-id="c57e3-115">The message body can be either HTML or text, with HTML as the default message body type returned in a GET response.</span></span>

<span data-ttu-id="c57e3-116">当[获取邮件](../api-reference/v1.0/api/message_get.md)时，你可以指定以下请求标头以文本格式返回 **body** 和 **uniqueBody** 属性：</span><span class="sxs-lookup"><span data-stu-id="c57e3-116">When [getting a message](../api-reference/v1.0/api/message_get.md), you can specify the following request header to return the **body** and **uniqueBody** properties in text format:</span></span>

```http
Prefer: outlook.body-content-type="text"
```

<span data-ttu-id="c57e3-117">你可以指定以下标头（或直接跳过标头），以 HTML 格式获取邮件正文：</span><span class="sxs-lookup"><span data-stu-id="c57e3-117">You can specify the following header, or, just skip the header, to get the message body in HTML format:</span></span>

```http
Prefer: outlook.body-content-type="html"
```

<span data-ttu-id="c57e3-118">当指定任一标头时，成功的响应将包含相应的 `Preference-Applied` 标头：</span><span class="sxs-lookup"><span data-stu-id="c57e3-118">When you specify either header, a successful response would include the corresponding `Preference-Applied` header:</span></span>

- <span data-ttu-id="c57e3-119">对于文本格式请求：`Preference-Applied: outlook.body-content-type="text"`</span><span class="sxs-lookup"><span data-stu-id="c57e3-119">For text format requests: `Preference-Applied: outlook.body-content-type="text"`</span></span>
- <span data-ttu-id="c57e3-120">对于 HTML 格式请求：`Preference-Applied: outlook.body-content-type="html"`</span><span class="sxs-lookup"><span data-stu-id="c57e3-120">For HTML format requests: `Preference-Applied: outlook.body-content-type="html"`</span></span>

<span data-ttu-id="c57e3-121">默认情况下，如果正文是 HTML 格式，那么在 REST 响应中返回正文内容之前，Outlook 将删除嵌入 **body** 属性中的任何具有潜在不安全性的 HTML（例如 JavaScript）。</span><span class="sxs-lookup"><span data-stu-id="c57e3-121">If the body is HTML, by default, Outlook removes any potentially unsafe HTML (for example, JavaScript) embedded in the **body** property before returning the body content in a REST response.</span></span>

<span data-ttu-id="c57e3-122">若要获取整个原始 HTML 内容，请包括以下 HTTP 请求标头：</span><span class="sxs-lookup"><span data-stu-id="c57e3-122">To get the entire, original HTML content, include the following HTTP request header:</span></span>

```http
Prefer: outlook.allow-unsafe-html
```

### <a name="differentiating-the-from-and-sender-properties"></a><span data-ttu-id="c57e3-123">区分 from 和 sender 属性</span><span class="sxs-lookup"><span data-stu-id="c57e3-123">Differentiating the from and sender properties</span></span>

<span data-ttu-id="c57e3-124">撰写邮件时，Outlook 在大多数情况下会将 **from** 和 **sender** 属性设置为同一登录用户。</span><span class="sxs-lookup"><span data-stu-id="c57e3-124">When a message is being composed, in most cases, Outlook sets the **from** and **sender** properties to the same signed-in user.</span></span> <span data-ttu-id="c57e3-125">你可以在以下情况下更新这些属性：</span><span class="sxs-lookup"><span data-stu-id="c57e3-125">You can update these properties in the following scenarios:</span></span>

- <span data-ttu-id="c57e3-p105">如果 Exchange 管理员已将邮箱的 **sendAs** 权限分配给其他一些用户，可以更改 **from** 属性。为此，管理员可以在 Azure 门户中选择邮箱所有者的**邮箱权限**，也可以使用 Exchange 管理中心或 Windows PowerShell Add-ADPermission cmdlet。然后，可以编程方式将 **from** 属性设置为，对相应邮箱拥有 **sendAs** 权限的用户之一。</span><span class="sxs-lookup"><span data-stu-id="c57e3-p105">The **from** property can be changed if the Exchange administrator has assigned **sendAs** rights of the mailbox to some other users. The administrator can do this by selecting **Mailbox Permissions** of the mailbox owner in the Azure portal, or by using the Exchange Admin Center or a Windows PowerShell Add-ADPermission cmdlet. Then, you can programmatically set the **from** property to one of these users who have **sendAs** rights for that mailbox.</span></span>
- <span data-ttu-id="c57e3-129">如果邮箱所有者已委派一个或多个用户能够从该邮箱发送邮件，则可以更改 **sender** 属性。</span><span class="sxs-lookup"><span data-stu-id="c57e3-129">The **sender** property can be changed if the mailbox owner has delegated one or more users to be able to send messages from that mailbox.</span></span> <span data-ttu-id="c57e3-130">可以在 Outlook 中委派邮箱所有者。</span><span class="sxs-lookup"><span data-stu-id="c57e3-130">The mailbox owner can delegate in Outlook.</span></span> <span data-ttu-id="c57e3-131">当代理代表邮箱所有者发送邮件时，Outlook 将 **sender** 属性设置为代理的帐户，**from** 属性仍保持为邮箱所有者。</span><span class="sxs-lookup"><span data-stu-id="c57e3-131">When a delegate sends a message on behalf of the mailbox owner, Outlook sets the **sender** property to the delegate’s account, and the **from** property remains as the mailbox owner.</span></span> <span data-ttu-id="c57e3-132">通过编程方式，你可以将 **sender** 属性设置为已拥有邮箱委派权限的用户。</span><span class="sxs-lookup"><span data-stu-id="c57e3-132">Programmatically, you can set the **sender** property to a user who has got delegate permissions for that mailbox.</span></span>

## <a name="using-mailtips-to-check-recipient-status-and-save-time-preview"></a><span data-ttu-id="c57e3-133">使用邮件提醒检查收件人状态并节省时间（预览版）</span><span class="sxs-lookup"><span data-stu-id="c57e3-133">Using MailTips to check recipient status and save time (preview)</span></span>

<span data-ttu-id="c57e3-134">在发送电子邮件之前，可使用[邮件提醒](../api-reference/beta/resources/mailtips.md)做出明智的决定。</span><span class="sxs-lookup"><span data-stu-id="c57e3-134">Use [MailTips](../api-reference/beta/resources/mailtips.md) to make smart decisions before sending an email.</span></span>
<span data-ttu-id="c57e3-135">邮件提醒可以告诉你诸如收件人的邮箱限于特定发件人，或者需要批准才能向收件人发送电子邮件等信息。</span><span class="sxs-lookup"><span data-stu-id="c57e3-135">MailTips can tell you information such as the recipient's mailbox is restricted to specific senders, or approval is required for emailing the recipient.</span></span>

## <a name="integrating-with--social-gesture-preview"></a><span data-ttu-id="c57e3-136">与“@”社交手势集成（预览版）</span><span class="sxs-lookup"><span data-stu-id="c57e3-136">Integrating with '@' social gesture (preview)</span></span>

<span data-ttu-id="c57e3-137">@-mention 是提醒用户邮件中是否有提到他们的通知。</span><span class="sxs-lookup"><span data-stu-id="c57e3-137">@-mentions are notifications to alert users if they are mentioned in messages.</span></span> <span data-ttu-id="c57e3-138">[mention](../api-reference/beta/resources/mention.md)资源使应用能够在电子邮件中设置和获取常见的在线社交手势，即“@”前缀。</span><span class="sxs-lookup"><span data-stu-id="c57e3-138">The [mention](../api-reference/beta/resources/mention.md) resource enables apps to set and get the common online social gesture, the '@' prefix, in emails.</span></span>
<span data-ttu-id="c57e3-139">可以执行下列操作：</span><span class="sxs-lookup"><span data-stu-id="c57e3-139">You can:</span></span>

- <span data-ttu-id="c57e3-140">在[创建邮件](../api-reference/beta/api/user_post_messages.md#request-2)时创建 @-mention</span><span class="sxs-lookup"><span data-stu-id="c57e3-140">Create @-mentions when [creating a message](../api-reference/beta/api/user_post_messages.md#request-2)</span></span>
- [<span data-ttu-id="c57e3-141">获取用户邮箱中包含用户 @-mention 的所有邮件</span><span class="sxs-lookup"><span data-stu-id="c57e3-141">Get all the messages in a user's mailbox that contain an @-mention of the user</span></span>](../api-reference/beta/api/user_list_messages.md#request-2)
- [<span data-ttu-id="c57e3-142">获取所有 @-mention 就形成一封邮件</span><span class="sxs-lookup"><span data-stu-id="c57e3-142">Get all the @-mention is a message</span></span>](../api-reference/beta/api/message_get.md#request-2)

## <a name="other-shared-capabilities"></a><span data-ttu-id="c57e3-143">其他共享的功能</span><span class="sxs-lookup"><span data-stu-id="c57e3-143">Other shared capabilities</span></span>

<span data-ttu-id="c57e3-144">利用以下在 Microsoft Graph 实体之间共享的常用功能：</span><span class="sxs-lookup"><span data-stu-id="c57e3-144">Take advantage of the following common capabilities that are shared among Microsoft Graph entities:</span></span>

- <span data-ttu-id="c57e3-145">发生一种或多种类型的更改时（如创建或更新邮件），订阅邮件的[更改通知](../api-reference/v1.0/resources/webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="c57e3-145">Subscribe to [change notifications](../api-reference/v1.0/resources/webhooks.md) on messages when one or more types of changes occur, such as message creation or update.</span></span>
- <span data-ttu-id="c57e3-146">[跟踪文件夹中邮件的这些增量更改](delta_query_messages.md)</span><span class="sxs-lookup"><span data-stu-id="c57e3-146">[Track these incremental changes to messages in a folder](delta_query_messages.md).</span></span>
- <span data-ttu-id="c57e3-147">创建[开放扩展](extensibility_overview.md#open-extensions)或[架构扩展](extensibility_overview.md#schema-extensions)，以将自定义数据添加到邮件实例。</span><span class="sxs-lookup"><span data-stu-id="c57e3-147">Create [open extensions](extensibility_overview.md#open-extensions) or [schema extensions](extensibility_overview.md#schema-extensions) to add custom data to a message instance.</span></span>
- <span data-ttu-id="c57e3-148">当 Outlook MAPI 属性尚未通过 Microsoft Graph API 元数据公开时，在邮件实例中创建[扩展属性](../api-reference/v1.0/resources/extended-properties-overview.md)以存储这些属性的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="c57e3-148">Create [extended properties](../api-reference/v1.0/resources/extended-properties-overview.md) in a message instance to store custom data for Outlook MAPI properties, when these properties are not already exposed in the Microsoft Graph API metadata.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c57e3-149">后续步骤</span><span class="sxs-lookup"><span data-stu-id="c57e3-149">Next steps</span></span>

<span data-ttu-id="c57e3-150">详细了解以下信息：</span><span class="sxs-lookup"><span data-stu-id="c57e3-150">Find out more about:</span></span>

- [<span data-ttu-id="c57e3-151">为什么与 Outlook 邮件集成</span><span class="sxs-lookup"><span data-stu-id="c57e3-151">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- <span data-ttu-id="c57e3-152">[使用邮件 API](../api-reference/v1.0/resources/mail_api_overview.md) 及其在 Microsoft Graph v1.0 中的[用例](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases)。</span><span class="sxs-lookup"><span data-stu-id="c57e3-152">[Using the mail API](../api-reference/v1.0/resources/mail_api_overview.md) and its [use cases](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases) in Microsoft Graph v1.0.</span></span>


<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error: /concepts/outlook-create-send-messages.md:
        BookmarkSkippedDocFileNotFound: Link '[creating a message](../api-reference/beta/api/user_post_messages.md#request-2)'.",
    "Error: /concepts/outlook-create-send-messages.md:
      BookmarkSkippedDocFileNotFound: Link '[Get all the messages in a user's mailbox that contain an @-mention of the user](../api-reference/beta/api/user_list_messages.md#request-2)'.",
    "Error: /concepts/outlook-create-send-messages.md:
      BookmarkSkippedDocFileNotFound: Link '[Get all the @-mention is a message](../api-reference/beta/api/message_get.md#request-2)'."
  ]
}-->
