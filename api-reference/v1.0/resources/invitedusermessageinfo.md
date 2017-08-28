# <a name="configuring-the-invitation-message"></a><span data-ttu-id="c07ce-101">配置邀请邮件</span><span class="sxs-lookup"><span data-stu-id="c07ce-101">Configuring the invitation message</span></span>

<span data-ttu-id="c07ce-102">使用 invitedUserMessageInfo 对象可以配置[邀请](invitation.md)邮件。</span><span class="sxs-lookup"><span data-stu-id="c07ce-102">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="c07ce-103">属性</span><span class="sxs-lookup"><span data-stu-id="c07ce-103">Properties</span></span>
| <span data-ttu-id="c07ce-104">属性</span><span class="sxs-lookup"><span data-stu-id="c07ce-104">Property</span></span>     | <span data-ttu-id="c07ce-105">类型</span><span class="sxs-lookup"><span data-stu-id="c07ce-105">Type</span></span>   |<span data-ttu-id="c07ce-106">说明</span><span class="sxs-lookup"><span data-stu-id="c07ce-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c07ce-107">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="c07ce-107">ccRecipients</span></span>|[<span data-ttu-id="c07ce-108">收件人</span><span class="sxs-lookup"><span data-stu-id="c07ce-108">Recipient</span></span>](recipient.md)|<span data-ttu-id="c07ce-p101">应接收邀请邮件的其他收件人。当前仅支持 1 个其他收件人。</span><span class="sxs-lookup"><span data-stu-id="c07ce-p101">Additional recipients the invitation message should be sent to. Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="c07ce-111">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="c07ce-111">customizedMessageBody</span></span>|<span data-ttu-id="c07ce-112">字符串</span><span class="sxs-lookup"><span data-stu-id="c07ce-112">String</span></span>|<span data-ttu-id="c07ce-113">在不希望发送默认邮件的情况下，要发送的自定义邮件正文。</span><span class="sxs-lookup"><span data-stu-id="c07ce-113">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="c07ce-114">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="c07ce-114">messageLanguage</span></span>|<span data-ttu-id="c07ce-115">字符串</span><span class="sxs-lookup"><span data-stu-id="c07ce-115">String</span></span>|<span data-ttu-id="c07ce-p102">要发送的默认邮件的语言。如果指定了 customizedMessageBody，则忽略此属性，并使用 customizedMessageBody 发送该邮件。语言格式应为 ISO 639 格式。默认为 zh-CN。</span><span class="sxs-lookup"><span data-stu-id="c07ce-p102">The language you want to send the default message in. If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody. The language format should be in ISO 639. The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c07ce-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c07ce-120">JSON representation</span></span>
<span data-ttu-id="c07ce-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c07ce-121">Here is a JSON representation of the resource</span></span>

<!-- {"blockType": "resource", "@odata.type": "microsoft.graph.invitedUserMessageInfo"} -->
```json
{
  "ccRecipients": [ {"@odata.type": "microsoft.graph.recipient"} ],
  "customizedMessageBody": "string",
  "messageLanguage": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2016-22-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "invitedUserMessageInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
