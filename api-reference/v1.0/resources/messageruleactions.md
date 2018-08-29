# <a name="messageruleactions-resource-type"></a><span data-ttu-id="d6516-101">messageRuleActions 资源类型</span><span class="sxs-lookup"><span data-stu-id="d6516-101">messageRuleActions resource type</span></span>


<span data-ttu-id="d6516-102">表示适用于规则的一组操作。</span><span class="sxs-lookup"><span data-stu-id="d6516-102">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="d6516-103">属性</span><span class="sxs-lookup"><span data-stu-id="d6516-103">Properties</span></span>
| <span data-ttu-id="d6516-104">属性</span><span class="sxs-lookup"><span data-stu-id="d6516-104">Property</span></span>     | <span data-ttu-id="d6516-105">类型</span><span class="sxs-lookup"><span data-stu-id="d6516-105">Type</span></span>   |<span data-ttu-id="d6516-106">说明</span><span class="sxs-lookup"><span data-stu-id="d6516-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d6516-107">assignCategories</span><span class="sxs-lookup"><span data-stu-id="d6516-107">assignCategories</span></span> | <span data-ttu-id="d6516-108">String 集合</span><span class="sxs-lookup"><span data-stu-id="d6516-108">String collection</span></span> | <span data-ttu-id="d6516-109">分配给邮件的类别列表。</span><span class="sxs-lookup"><span data-stu-id="d6516-109">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="d6516-110">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="d6516-110">copyToFolder</span></span> | <span data-ttu-id="d6516-111">String</span><span class="sxs-lookup"><span data-stu-id="d6516-111">String</span></span> | <span data-ttu-id="d6516-112">将邮件复制到其中的文件夹的 ID。</span><span class="sxs-lookup"><span data-stu-id="d6516-112">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="d6516-113">delete</span><span class="sxs-lookup"><span data-stu-id="d6516-113">delete</span></span> | <span data-ttu-id="d6516-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6516-114">Boolean</span></span> | <span data-ttu-id="d6516-115">指示邮件是否应移动到“已删除项目”文件夹。</span><span class="sxs-lookup"><span data-stu-id="d6516-115">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="d6516-116">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="d6516-116">forwardAsAttachmentTo</span></span> | <span data-ttu-id="d6516-117">[recipient](recipient.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d6516-117">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="d6516-118">应以附件形式接收转发邮件的收件人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="d6516-118">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="d6516-119">forwardTo</span><span class="sxs-lookup"><span data-stu-id="d6516-119">forwardTo</span></span> | <span data-ttu-id="d6516-120">[recipient](recipient.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d6516-120">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="d6516-121">应接收转发邮件的收件人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="d6516-121">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="d6516-122">markAsRead</span><span class="sxs-lookup"><span data-stu-id="d6516-122">markAsRead</span></span> | <span data-ttu-id="d6516-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6516-123">Boolean</span></span> | <span data-ttu-id="d6516-124">指示是否应将邮件标记为已读。</span><span class="sxs-lookup"><span data-stu-id="d6516-124">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="d6516-125">markImportance</span><span class="sxs-lookup"><span data-stu-id="d6516-125">markImportance</span></span> | <span data-ttu-id="d6516-126">importance</span><span class="sxs-lookup"><span data-stu-id="d6516-126">importance</span></span> | <span data-ttu-id="d6516-127">设置邮件重要性，可以是：`low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="d6516-127">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="d6516-128">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="d6516-128">moveToFolder</span></span> |  <span data-ttu-id="d6516-129">String</span><span class="sxs-lookup"><span data-stu-id="d6516-129">String</span></span>| <span data-ttu-id="d6516-130">邮件将移至其中的文件夹的 ID。</span><span class="sxs-lookup"><span data-stu-id="d6516-130">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="d6516-131">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="d6516-131">permanentDelete</span></span> | <span data-ttu-id="d6516-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6516-132">Boolean</span></span> | <span data-ttu-id="d6516-133">指示邮件是否应永久删除且不保存到“已删除项目”文件夹。</span><span class="sxs-lookup"><span data-stu-id="d6516-133">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="d6516-134">redirectTo</span><span class="sxs-lookup"><span data-stu-id="d6516-134">redirectTo</span></span> | <span data-ttu-id="d6516-135">[recipient](recipient.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d6516-135">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="d6516-136">邮件应重定向到的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="d6516-136">The email address to which a message should be redirected.</span></span> |
| <span data-ttu-id="d6516-137">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="d6516-137">stopProcessingRules</span></span> | <span data-ttu-id="d6516-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6516-138">Boolean</span></span> | <span data-ttu-id="d6516-139">指示是否应对后续规则进行评估。</span><span class="sxs-lookup"><span data-stu-id="d6516-139">Indicates whether subsequent rules should be evaluated.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d6516-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d6516-140">JSON representation</span></span>
<span data-ttu-id="d6516-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6516-141">Here is a JSON representation of the resource.</span></span>

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
  "redirectTo": [{"@odata.type": "microsoft.graph.recipient"}],
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