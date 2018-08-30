# <a name="inferenceclassification-resource-type"></a><span data-ttu-id="70e7a-101">inferenceClassification 资源类型</span><span class="sxs-lookup"><span data-stu-id="70e7a-101">inferenceClassification resource type</span></span>

<span data-ttu-id="70e7a-102">用户邮件分类，确保仅关注对用户更相关或更重要的邮件。</span><span class="sxs-lookup"><span data-stu-id="70e7a-102">Classification of a user's messages to enable focus on those that are more relevant or important to the user.</span></span> 

<span data-ttu-id="70e7a-103">有关详细信息，请参阅 [管理重点收件箱](manage_focused_inbox.md)。</span><span class="sxs-lookup"><span data-stu-id="70e7a-103">For more information, see [Manage Focused Inbox](manage_focused_inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="70e7a-104">方法</span><span class="sxs-lookup"><span data-stu-id="70e7a-104">Methods</span></span>

| <span data-ttu-id="70e7a-105">方法</span><span class="sxs-lookup"><span data-stu-id="70e7a-105">Method</span></span>           | <span data-ttu-id="70e7a-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="70e7a-106">Return Type</span></span>    |<span data-ttu-id="70e7a-107">说明</span><span class="sxs-lookup"><span data-stu-id="70e7a-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="70e7a-108">Create inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="70e7a-108">Create inferenceClassificationOverride</span></span>](../api/inferenceclassification_post_overrides.md) |[<span data-ttu-id="70e7a-109">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="70e7a-109">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md)| <span data-ttu-id="70e7a-p101">创建由 SMTP 地址识别的发件人的替代。将以后来自该 SMTP 地址的邮件一致归为替代中指定的类别。</span><span class="sxs-lookup"><span data-stu-id="70e7a-p101">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>|
|[<span data-ttu-id="70e7a-112">List overrides</span><span class="sxs-lookup"><span data-stu-id="70e7a-112">List overrides</span></span>](../api/inferenceclassification_list_overrides.md) |<span data-ttu-id="70e7a-113">[inferenceClassificationOverride](inferenceclassificationoverride.md) 集合</span><span class="sxs-lookup"><span data-stu-id="70e7a-113">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="70e7a-114">获取用户设置为始终以特定方式对来自特定发件人的邮件进行分类的替代。</span><span class="sxs-lookup"><span data-stu-id="70e7a-114">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>|

## <a name="properties"></a><span data-ttu-id="70e7a-115">属性</span><span class="sxs-lookup"><span data-stu-id="70e7a-115">Properties</span></span>
| <span data-ttu-id="70e7a-116">属性</span><span class="sxs-lookup"><span data-stu-id="70e7a-116">Property</span></span>     | <span data-ttu-id="70e7a-117">类型</span><span class="sxs-lookup"><span data-stu-id="70e7a-117">Type</span></span>   |<span data-ttu-id="70e7a-118">说明</span><span class="sxs-lookup"><span data-stu-id="70e7a-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70e7a-119">id</span><span class="sxs-lookup"><span data-stu-id="70e7a-119">id</span></span>|<span data-ttu-id="70e7a-120">string</span><span class="sxs-lookup"><span data-stu-id="70e7a-120">string</span></span>| <span data-ttu-id="70e7a-121">只读。</span><span class="sxs-lookup"><span data-stu-id="70e7a-121">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="70e7a-122">关系</span><span class="sxs-lookup"><span data-stu-id="70e7a-122">Relationships</span></span>
| <span data-ttu-id="70e7a-123">关系</span><span class="sxs-lookup"><span data-stu-id="70e7a-123">Relationship</span></span> | <span data-ttu-id="70e7a-124">类型</span><span class="sxs-lookup"><span data-stu-id="70e7a-124">Type</span></span>   |<span data-ttu-id="70e7a-125">说明</span><span class="sxs-lookup"><span data-stu-id="70e7a-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70e7a-126">overrides</span><span class="sxs-lookup"><span data-stu-id="70e7a-126">overrides</span></span>|<span data-ttu-id="70e7a-127">[inferenceClassificationOverride](inferenceclassificationoverride.md) 集合</span><span class="sxs-lookup"><span data-stu-id="70e7a-127">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="70e7a-p102">用户始终按某种方式（`focused` 或 `other`）对来自特定发件人的邮件分类的一组替代。只读。可为 null。</span><span class="sxs-lookup"><span data-stu-id="70e7a-p102">A set of overrides for a user to always classify messages from specific senders in certain ways: `focused`, or `other`. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="70e7a-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="70e7a-131">JSON representation</span></span>

<span data-ttu-id="70e7a-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="70e7a-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.inferenceClassification",
  "@odata.annotations": [
    {
      "property": "overrides",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->