# <a name="channel-resource-type"></a><span data-ttu-id="eb0cb-101">通道资源类型</span><span class="sxs-lookup"><span data-stu-id="eb0cb-101">channel resource type</span></span>



<span data-ttu-id="eb0cb-102">频道是[团队](../resources/team.md)中的邮件的集合。</span><span class="sxs-lookup"><span data-stu-id="eb0cb-102">A channel is a collection of messages within a [team](../resources/team.md).</span></span> <span data-ttu-id="eb0cb-103">通道表示一个主题，因此讨论，团队中的逻辑隔离。</span><span class="sxs-lookup"><span data-stu-id="eb0cb-103">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="eb0cb-104">示例可以是"星期五团队可边午餐"通道和"体系结构讨论"通道。</span><span class="sxs-lookup"><span data-stu-id="eb0cb-104">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="eb0cb-105">方法</span><span class="sxs-lookup"><span data-stu-id="eb0cb-105">Methods</span></span>

| <span data-ttu-id="eb0cb-106">方法</span><span class="sxs-lookup"><span data-stu-id="eb0cb-106">Method</span></span>       | <span data-ttu-id="eb0cb-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="eb0cb-107">Return Type</span></span>  |<span data-ttu-id="eb0cb-108">说明</span><span class="sxs-lookup"><span data-stu-id="eb0cb-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eb0cb-109">列表通道</span><span class="sxs-lookup"><span data-stu-id="eb0cb-109">List channels</span></span>](../api/channel_list.md) | <span data-ttu-id="eb0cb-110">[通道](channel.md)集合</span><span class="sxs-lookup"><span data-stu-id="eb0cb-110">[channel](channel.md) collection</span></span> | <span data-ttu-id="eb0cb-111">此团队中获取通道的列表。</span><span class="sxs-lookup"><span data-stu-id="eb0cb-111">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="eb0cb-112">创建通道</span><span class="sxs-lookup"><span data-stu-id="eb0cb-112">Create channel</span></span>](../api/channel_post.md) | [<span data-ttu-id="eb0cb-113">通道</span><span class="sxs-lookup"><span data-stu-id="eb0cb-113">channel</span></span>](channel.md) | <span data-ttu-id="eb0cb-114">创建新的通道通过包括的显示名称和说明。</span><span class="sxs-lookup"><span data-stu-id="eb0cb-114">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="eb0cb-115">获取通道</span><span class="sxs-lookup"><span data-stu-id="eb0cb-115">Get channel</span></span>](../api/channel_get.md) | [<span data-ttu-id="eb0cb-116">通道</span><span class="sxs-lookup"><span data-stu-id="eb0cb-116">channel</span></span>](channel.md) | <span data-ttu-id="eb0cb-117">读取属性和该频道的关系。</span><span class="sxs-lookup"><span data-stu-id="eb0cb-117">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="eb0cb-118">更新通道</span><span class="sxs-lookup"><span data-stu-id="eb0cb-118">Update channel</span></span>](../api/channel_patch.md) | [<span data-ttu-id="eb0cb-119">通道</span><span class="sxs-lookup"><span data-stu-id="eb0cb-119">channel</span></span>](channel.md) | <span data-ttu-id="eb0cb-120">更新该频道的属性。</span><span class="sxs-lookup"><span data-stu-id="eb0cb-120">Update properties of the channel.</span></span>|
|[<span data-ttu-id="eb0cb-121">删除通道</span><span class="sxs-lookup"><span data-stu-id="eb0cb-121">Delete channel</span></span>](../api/channel_delete.md) | <span data-ttu-id="eb0cb-122">无</span><span class="sxs-lookup"><span data-stu-id="eb0cb-122">None</span></span> | <span data-ttu-id="eb0cb-123">删除通道。</span><span class="sxs-lookup"><span data-stu-id="eb0cb-123">Delete a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="eb0cb-124">属性</span><span class="sxs-lookup"><span data-stu-id="eb0cb-124">Properties</span></span>
| <span data-ttu-id="eb0cb-125">属性</span><span class="sxs-lookup"><span data-stu-id="eb0cb-125">Property</span></span>     | <span data-ttu-id="eb0cb-126">类型</span><span class="sxs-lookup"><span data-stu-id="eb0cb-126">Type</span></span>   |<span data-ttu-id="eb0cb-127">说明</span><span class="sxs-lookup"><span data-stu-id="eb0cb-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb0cb-128">说明</span><span class="sxs-lookup"><span data-stu-id="eb0cb-128">description</span></span>|<span data-ttu-id="eb0cb-129">字符串</span><span class="sxs-lookup"><span data-stu-id="eb0cb-129">String</span></span>|<span data-ttu-id="eb0cb-130">通道的可选文字说明。</span><span class="sxs-lookup"><span data-stu-id="eb0cb-130">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="eb0cb-131">displayName</span><span class="sxs-lookup"><span data-stu-id="eb0cb-131">displayName</span></span>|<span data-ttu-id="eb0cb-132">字符串</span><span class="sxs-lookup"><span data-stu-id="eb0cb-132">String</span></span>|<span data-ttu-id="eb0cb-133">通道名称将显示于 Microsoft 团队中的用户。</span><span class="sxs-lookup"><span data-stu-id="eb0cb-133">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="eb0cb-134">id</span><span class="sxs-lookup"><span data-stu-id="eb0cb-134">id</span></span>|<span data-ttu-id="eb0cb-135">字符串</span><span class="sxs-lookup"><span data-stu-id="eb0cb-135">String</span></span>|<span data-ttu-id="eb0cb-136">通道的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="eb0cb-136">The channels's unique identifier.</span></span> <span data-ttu-id="eb0cb-137">只读。</span><span class="sxs-lookup"><span data-stu-id="eb0cb-137">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb0cb-138">Relationships</span><span class="sxs-lookup"><span data-stu-id="eb0cb-138">Relationships</span></span>
| <span data-ttu-id="eb0cb-139">关系</span><span class="sxs-lookup"><span data-stu-id="eb0cb-139">Relationship</span></span> | <span data-ttu-id="eb0cb-140">类型</span><span class="sxs-lookup"><span data-stu-id="eb0cb-140">Type</span></span>   |<span data-ttu-id="eb0cb-141">说明</span><span class="sxs-lookup"><span data-stu-id="eb0cb-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb0cb-142">选项卡</span><span class="sxs-lookup"><span data-stu-id="eb0cb-142">tabs</span></span>|<span data-ttu-id="eb0cb-143">[teamsTab](../resources/teamstab.md)集合</span><span class="sxs-lookup"><span data-stu-id="eb0cb-143">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="eb0cb-144">在进入频道的所有选项卡的集合。</span><span class="sxs-lookup"><span data-stu-id="eb0cb-144">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="eb0cb-145">导航属性。</span><span class="sxs-lookup"><span data-stu-id="eb0cb-145">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="eb0cb-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eb0cb-146">JSON representation</span></span>

<span data-ttu-id="eb0cb-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb0cb-147">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "chatthreads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
