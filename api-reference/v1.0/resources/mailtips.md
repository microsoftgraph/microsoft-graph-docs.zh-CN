# <a name="mailtips-resource-type"></a><span data-ttu-id="51323-101">邮件提醒资源类型</span><span class="sxs-lookup"><span data-stu-id="51323-101">mailTips resource type</span></span>

<span data-ttu-id="51323-102">有关收件人的提示消息，用户撰写消息时向用户显示。</span><span class="sxs-lookup"><span data-stu-id="51323-102">Informative messages displayed to users while they are composing a message.</span></span> <span data-ttu-id="51323-103">例如，将外出邮件作为邮件收件人的自动答复。</span><span class="sxs-lookup"><span data-stu-id="51323-103">For example, an out-of-office message as an automatic reply for a message recipient.</span></span>


## <a name="properties"></a><span data-ttu-id="51323-104">属性</span><span class="sxs-lookup"><span data-stu-id="51323-104">Properties</span></span>
| <span data-ttu-id="51323-105">属性</span><span class="sxs-lookup"><span data-stu-id="51323-105">Property</span></span>     | <span data-ttu-id="51323-106">类型</span><span class="sxs-lookup"><span data-stu-id="51323-106">Type</span></span>   |<span data-ttu-id="51323-107">说明</span><span class="sxs-lookup"><span data-stu-id="51323-107">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="51323-108">AutomaticReplies</span><span class="sxs-lookup"><span data-stu-id="51323-108">AutomaticReplies</span></span> | [<span data-ttu-id="51323-109">AutomaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="51323-109">AutomaticRepliesMailTips</span></span>](../resources/automaticrepliesmailtips.md) | <span data-ttu-id="51323-110">邮件提示自动答复（如果它已由收件人设置）。</span><span class="sxs-lookup"><span data-stu-id="51323-110">Mail tips for automatic reply if it has been set up by the recipient.</span></span> |
| <span data-ttu-id="51323-111">CustomMailTip</span><span class="sxs-lookup"><span data-stu-id="51323-111">CustomMailTip</span></span> | <span data-ttu-id="51323-112">字符串</span><span class="sxs-lookup"><span data-stu-id="51323-112">String</span></span> | <span data-ttu-id="51323-113">可以在收件人的邮箱上设置的自定义邮件提示。</span><span class="sxs-lookup"><span data-stu-id="51323-113">A custom mail tip that can be set on the recipient's mailbox.</span></span> |
| <span data-ttu-id="51323-114">DeliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="51323-114">DeliveryRestricted</span></span>| <span data-ttu-id="51323-115">布尔值</span><span class="sxs-lookup"><span data-stu-id="51323-115">Boolean</span></span> | <span data-ttu-id="51323-116">收件人的邮箱是否受限制，例如仅接受来自预定义的发件人列表的邮件，拒绝来自预定义的发件人列表的邮件，或仅接受来自经过验证的发件人的邮件。</span><span class="sxs-lookup"><span data-stu-id="51323-116">Whether the recipient's mailbox is restricted, for example, accepting messages from only a predefined list of senders, rejecting messages from a predefined list of senders, or accepting messages from only authenticated senders.</span></span> |
| <span data-ttu-id="51323-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="51323-117">emailAddress</span></span> | [<span data-ttu-id="51323-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="51323-118">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="51323-119">收件人的邮件地址以获取邮件提醒。</span><span class="sxs-lookup"><span data-stu-id="51323-119">The email address of the recipient to get mailtips for.</span></span> |
| <span data-ttu-id="51323-120">error</span><span class="sxs-lookup"><span data-stu-id="51323-120">error</span></span> | [<span data-ttu-id="51323-121">mailTipsError</span><span class="sxs-lookup"><span data-stu-id="51323-121">mailTipsError</span></span>](../resources/mailtipserror.md) | <span data-ttu-id="51323-122">在 [GetMailTips](../api/user_getmailtips.md) 操作期间发生的错误。</span><span class="sxs-lookup"><span data-stu-id="51323-122">Errors that occur during the [GetMailTips](../api/user_getmailtips.md) action.</span></span> |
| <span data-ttu-id="51323-123">ExternalMemberCount</span><span class="sxs-lookup"><span data-stu-id="51323-123">ExternalMemberCount</span></span> | <span data-ttu-id="51323-124">Int32</span><span class="sxs-lookup"><span data-stu-id="51323-124">Int32</span></span> | <span data-ttu-id="51323-125">外部成员的数量（如果收件人为通讯组列表）。</span><span class="sxs-lookup"><span data-stu-id="51323-125">The number of external members if the recipient is a distribution list.</span></span> |
| <span data-ttu-id="51323-126">isModerated</span><span class="sxs-lookup"><span data-stu-id="51323-126">IsModerated</span></span> |<span data-ttu-id="51323-127">布尔值</span><span class="sxs-lookup"><span data-stu-id="51323-127">Boolean</span></span>  | <span data-ttu-id="51323-128">是否向收件人发送邮件需要批准。</span><span class="sxs-lookup"><span data-stu-id="51323-128">Whether sending messages to the recipient requires approval.</span></span> <span data-ttu-id="51323-129">例如，如果收件人是大型通讯组列表，并且主持人已设置为批准发送到该通讯组列表的邮件，或者如果向收件人发送邮件需要收件人的经理批准。</span><span class="sxs-lookup"><span data-stu-id="51323-129">For example, if the recipient is a large distribution list and a moderator has been set up to approve messages sent to that distribution list, or if sending messages to a recipient requires approval of the recipient's manager.</span></span> |
| <span data-ttu-id="51323-130">MailboxFull</span><span class="sxs-lookup"><span data-stu-id="51323-130">MailboxFull</span></span> | <span data-ttu-id="51323-131">布尔值</span><span class="sxs-lookup"><span data-stu-id="51323-131">Boolean</span></span> | <span data-ttu-id="51323-132">收件人邮箱的完整状态。</span><span class="sxs-lookup"><span data-stu-id="51323-132">The mailbox full status of the recipient.</span></span> |
| <span data-ttu-id="51323-133">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="51323-133">MaxMessageSize</span></span> | <span data-ttu-id="51323-134">Int32</span><span class="sxs-lookup"><span data-stu-id="51323-134">Int32</span></span> | <span data-ttu-id="51323-135">为收件人的组织或邮箱配置的最大邮件大小。</span><span class="sxs-lookup"><span data-stu-id="51323-135">The maximum message size that has been configured for the recipient's organization or mailbox.</span></span> |
| <span data-ttu-id="51323-136">RecipientScope</span><span class="sxs-lookup"><span data-stu-id="51323-136">RecipientScope</span></span> | <span data-ttu-id="51323-137">recipientScopeType</span><span class="sxs-lookup"><span data-stu-id="51323-137">RecipientScopeType</span></span> | <span data-ttu-id="51323-138">收件人的作用域。</span><span class="sxs-lookup"><span data-stu-id="51323-138">The scope of the recipient, such as internal, external, partner.</span></span> <span data-ttu-id="51323-139">可取值为：`none`、`internal`、`external`、`externalPartner`、`externalNonParther`。</span><span class="sxs-lookup"><span data-stu-id="51323-139">Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span></span> <span data-ttu-id="51323-140">例如，管理员可以将另一个组织设置为其“合作伙伴”。</span><span class="sxs-lookup"><span data-stu-id="51323-140">For example, an administrator can set another organization to be its "partner".</span></span> <span data-ttu-id="51323-141">如果管理员希望特定范围的用户可以访问某些邮件提醒，该范围很有用。</span><span class="sxs-lookup"><span data-stu-id="51323-141">The scope is useful if an administrator wants certain mailtips to be accessible to certain scopes.</span></span> <span data-ttu-id="51323-142">发件人可以告诉他们，他们的邮件可能会发送至组织以外的收件人，从而帮助他们做出关于措辞、语调和内容的正确决定。</span><span class="sxs-lookup"><span data-stu-id="51323-142">It's also useful to senders to inform them that their message may leave the organization, helping them make the correct decisions about wording, tone and content.</span></span>|
| <span data-ttu-id="51323-143">RecipientSuggestions</span><span class="sxs-lookup"><span data-stu-id="51323-143">RecipientSuggestions</span></span> | <span data-ttu-id="51323-144">[收件人](../resources/recipient.md) 集合</span><span class="sxs-lookup"><span data-stu-id="51323-144">[recipient](../resources/recipient.md) collection</span></span> | <span data-ttu-id="51323-145">基于此前上下文所建议的收件人，它们出现在相同的邮件中。</span><span class="sxs-lookup"><span data-stu-id="51323-145">Recipients suggested based on previous contexts where they appear in the same message.</span></span> |
| <span data-ttu-id="51323-146">TotalMemberCount</span><span class="sxs-lookup"><span data-stu-id="51323-146">TotalMemberCount</span></span> | <span data-ttu-id="51323-147">Int32</span><span class="sxs-lookup"><span data-stu-id="51323-147">Int32</span></span> | <span data-ttu-id="51323-148">收件人是通讯组列表的成员数量。</span><span class="sxs-lookup"><span data-stu-id="51323-148">The number of members if the recipient is a distribution list.</span></span> |

### <a name="recipientscopetype-values"></a><span data-ttu-id="51323-149">recipientScopeType 值</span><span class="sxs-lookup"><span data-stu-id="51323-149">recipientScopeType values</span></span>

| <span data-ttu-id="51323-150">值</span><span class="sxs-lookup"><span data-stu-id="51323-150">Value</span></span>
|:-------------------------
| <span data-ttu-id="51323-151">none</span><span class="sxs-lookup"><span data-stu-id="51323-151">none</span></span>
| <span data-ttu-id="51323-152">internal</span><span class="sxs-lookup"><span data-stu-id="51323-152">Internal</span></span>
| <span data-ttu-id="51323-153">external</span><span class="sxs-lookup"><span data-stu-id="51323-153">External</span></span>
| <span data-ttu-id="51323-154">externalPartner</span><span class="sxs-lookup"><span data-stu-id="51323-154">ExternalPartner</span></span>
| <span data-ttu-id="51323-155">externalNonPartner</span><span class="sxs-lookup"><span data-stu-id="51323-155">ExternalNonPartner</span></span>


## <a name="json-representation"></a><span data-ttu-id="51323-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="51323-156">JSON representation</span></span>

<span data-ttu-id="51323-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51323-157">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "automaticReplies",
    "customMailTip",
    "deliveryRestricted",
    "emailAddress",
    "error",
    "externalMemberCount",
    "isModerated",
    "mailboxFull",
    "maxMessageSize",
    "recipientScope",
    "recipientSuggestions",
    "totalMemberCount"
  ],
  "@odata.type": "microsoft.graph.mailTips"
}-->

```json
{
  "automaticReplies": {"@odata.type": "microsoft.graph.automaticRepliesMailTips"},
  "customMailTip": "string",
  "deliveryRestricted": "boolean",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"},
  "error": {"@odata.type": "microsoft.graph.mailTipsError"},
  "externalMemberCount": 1024,
  "isModerated": "boolean",
  "mailboxFull": "boolean",
  "maxMessageSize": 1024,
  "recipientScope": "string",
  "recipientSuggestions": [{"@odata.type": "microsoft.graph.recipient"}],
  "totalMemberCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailtips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
