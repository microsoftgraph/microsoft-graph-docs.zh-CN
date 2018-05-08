# <a name="messageruleactions-resource-type"></a><span data-ttu-id="9e773-101">messageRuleActions 资源类型</span><span class="sxs-lookup"><span data-stu-id="9e773-101">messageRuleActions resource type</span></span>


<span data-ttu-id="9e773-102">表示适用于规则的一组操作。</span><span class="sxs-lookup"><span data-stu-id="9e773-102">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="9e773-103">属性</span><span class="sxs-lookup"><span data-stu-id="9e773-103">Properties</span></span>
| <span data-ttu-id="9e773-104">属性</span><span class="sxs-lookup"><span data-stu-id="9e773-104">Property</span></span>     | <span data-ttu-id="9e773-105">类型</span><span class="sxs-lookup"><span data-stu-id="9e773-105">Type</span></span>   |<span data-ttu-id="9e773-106">说明</span><span class="sxs-lookup"><span data-stu-id="9e773-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9e773-107">assignCategories</span><span class="sxs-lookup"><span data-stu-id="9e773-107">assignCategories</span></span> | <span data-ttu-id="9e773-108">String 集合</span><span class="sxs-lookup"><span data-stu-id="9e773-108">String collection</span></span> | <span data-ttu-id="9e773-109">分配给邮件的类别列表。</span><span class="sxs-lookup"><span data-stu-id="9e773-109">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="9e773-110">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="9e773-110">copyToFolder</span></span> | <span data-ttu-id="9e773-111">String</span><span class="sxs-lookup"><span data-stu-id="9e773-111">String</span></span> | <span data-ttu-id="9e773-112">将邮件复制到其中的文件夹的 ID。</span><span class="sxs-lookup"><span data-stu-id="9e773-112">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="9e773-113">delete</span><span class="sxs-lookup"><span data-stu-id="9e773-113">delete</span></span> | <span data-ttu-id="9e773-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e773-114">Boolean</span></span> | <span data-ttu-id="9e773-115">指示邮件是否应移动到“已删除项目”文件夹。</span><span class="sxs-lookup"><span data-stu-id="9e773-115">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="9e773-116">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="9e773-116">forwardAsAttachmentTo</span></span> | <span data-ttu-id="9e773-117">[recipient](recipient.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9e773-117">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="9e773-118">应以附件形式接收转发邮件的收件人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="9e773-118">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="9e773-119">forwardTo</span><span class="sxs-lookup"><span data-stu-id="9e773-119">forwardTo</span></span> | <span data-ttu-id="9e773-120">[recipient](recipient.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9e773-120">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="9e773-121">应接收转发邮件的收件人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="9e773-121">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="9e773-122">markAsRead</span><span class="sxs-lookup"><span data-stu-id="9e773-122">markAsRead</span></span> | <span data-ttu-id="9e773-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e773-123">Boolean</span></span> | <span data-ttu-id="9e773-124">指示是否应将邮件标记为已读。</span><span class="sxs-lookup"><span data-stu-id="9e773-124">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="9e773-125">markImportance</span><span class="sxs-lookup"><span data-stu-id="9e773-125">markImportance</span></span> | <span data-ttu-id="9e773-126">String</span><span class="sxs-lookup"><span data-stu-id="9e773-126">String</span></span> | <span data-ttu-id="9e773-127">设置邮件重要性，可以是：`low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="9e773-127">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="9e773-128">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="9e773-128">moveToFolder</span></span> |  <span data-ttu-id="9e773-129">String</span><span class="sxs-lookup"><span data-stu-id="9e773-129">String</span></span>| <span data-ttu-id="9e773-130">邮件将移至其中的文件夹的 ID。</span><span class="sxs-lookup"><span data-stu-id="9e773-130">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="9e773-131">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="9e773-131">permanentDelete</span></span> | <span data-ttu-id="9e773-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e773-132">Boolean</span></span> | <span data-ttu-id="9e773-133">指示邮件是否应永久删除且不保存到“已删除项目”文件夹。</span><span class="sxs-lookup"><span data-stu-id="9e773-133">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="9e773-134">redirectTo</span><span class="sxs-lookup"><span data-stu-id="9e773-134">redirectTo</span></span> | [<span data-ttu-id="9e773-135">recipient</span><span class="sxs-lookup"><span data-stu-id="9e773-135">recipient</span></span>](recipient.md) | <span data-ttu-id="9e773-136">邮件应重定向到的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="9e773-136">The email address to which a message should be redirected.</span></span> |
| <span data-ttu-id="9e773-137">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="9e773-137">stopProcessingRules</span></span> | <span data-ttu-id="9e773-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e773-138">Boolean</span></span> | <span data-ttu-id="9e773-139">指示是否应对后续规则进行评估。</span><span class="sxs-lookup"><span data-stu-id="9e773-139">Indicates whether subsequent rules should be evaluated.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="9e773-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9e773-140">JSON representation</span></span>
<span data-ttu-id="9e773-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e773-141">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.messageRuleActions"
}-->

```json
{
  "assignCategories": ["String"],
  "copyToFolder": "String",
  "delete": "Boolean",
  "forwardAsAttachmentTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "forwardTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "markAsRead": "Boolean",
  "markImportance": "String",
  "moveToFolder": "String",
  "permanentDelete": "Boolean",
  "redirectTo": {"@odata.type": "microsoft.graph.recipient"},
  "stopProcessingRules": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRuleActions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->