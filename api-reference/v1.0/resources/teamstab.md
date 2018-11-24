# <a name="teamstab-resource-type"></a><span data-ttu-id="9f616-101">teamsTab 资源类型</span><span class="sxs-lookup"><span data-stu-id="9f616-101">teamsTab resource type</span></span>



<span data-ttu-id="9f616-102">TeamsTab 是[选项卡上](../resources/teamstab.md)的具有固定 （附加） 到[团队](team.md)内的[通道](channel.md)。</span><span class="sxs-lookup"><span data-stu-id="9f616-102">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="9f616-103">方法</span><span class="sxs-lookup"><span data-stu-id="9f616-103">Methods</span></span>

| <span data-ttu-id="9f616-104">方法</span><span class="sxs-lookup"><span data-stu-id="9f616-104">Method</span></span>       | <span data-ttu-id="9f616-105">返回类型</span><span class="sxs-lookup"><span data-stu-id="9f616-105">Return Type</span></span>  |<span data-ttu-id="9f616-106">说明</span><span class="sxs-lookup"><span data-stu-id="9f616-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9f616-107">列表选项卡</span><span class="sxs-lookup"><span data-stu-id="9f616-107">List tabs</span></span>](../api/teamstab_list.md) | [<span data-ttu-id="9f616-108">teamsTab</span><span class="sxs-lookup"><span data-stu-id="9f616-108">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="9f616-109">到通道固定列表选项卡。</span><span class="sxs-lookup"><span data-stu-id="9f616-109">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="9f616-110">获取选项卡</span><span class="sxs-lookup"><span data-stu-id="9f616-110">Get tab</span></span>](../api/teamstab_get.md) | [<span data-ttu-id="9f616-111">teamsTab</span><span class="sxs-lookup"><span data-stu-id="9f616-111">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="9f616-112">读取固定到频道的一个选项卡。</span><span class="sxs-lookup"><span data-stu-id="9f616-112">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="9f616-113">添加选项卡</span><span class="sxs-lookup"><span data-stu-id="9f616-113">Add tab</span></span>](../api/teamstab_add.md) | [<span data-ttu-id="9f616-114">teamsTab</span><span class="sxs-lookup"><span data-stu-id="9f616-114">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="9f616-115">添加 (pin) 通道向选项卡。</span><span class="sxs-lookup"><span data-stu-id="9f616-115">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="9f616-116">删除选项卡</span><span class="sxs-lookup"><span data-stu-id="9f616-116">Remove tab</span></span>](../api/teamstab_delete.md) | <span data-ttu-id="9f616-117">无</span><span class="sxs-lookup"><span data-stu-id="9f616-117">None</span></span> | <span data-ttu-id="9f616-118">删除 （取消锁定） 通道从选项卡。</span><span class="sxs-lookup"><span data-stu-id="9f616-118">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="9f616-119">更新选项卡</span><span class="sxs-lookup"><span data-stu-id="9f616-119">Update tab</span></span>](../api/teamstab_update.md) | [<span data-ttu-id="9f616-120">teamsTab</span><span class="sxs-lookup"><span data-stu-id="9f616-120">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="9f616-121">更新选项卡属性。</span><span class="sxs-lookup"><span data-stu-id="9f616-121">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="9f616-122">属性</span><span class="sxs-lookup"><span data-stu-id="9f616-122">Properties</span></span>

|<span data-ttu-id="9f616-123">属性</span><span class="sxs-lookup"><span data-stu-id="9f616-123">Property</span></span>|<span data-ttu-id="9f616-124">类型</span><span class="sxs-lookup"><span data-stu-id="9f616-124">Type</span></span>|<span data-ttu-id="9f616-125">说明</span><span class="sxs-lookup"><span data-stu-id="9f616-125">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="9f616-126">ID</span><span class="sxs-lookup"><span data-stu-id="9f616-126">id</span></span>              |   <span data-ttu-id="9f616-127">string</span><span class="sxs-lookup"><span data-stu-id="9f616-127">string</span></span>                  |  <span data-ttu-id="9f616-128">唯一标识通道选项读取仅的特定实例的标识符。</span><span class="sxs-lookup"><span data-stu-id="9f616-128">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="9f616-129">displayName</span><span class="sxs-lookup"><span data-stu-id="9f616-129">displayName</span></span>            |   <span data-ttu-id="9f616-130">string</span><span class="sxs-lookup"><span data-stu-id="9f616-130">string</span></span>                  |  <span data-ttu-id="9f616-131">Tab 的名称。</span><span class="sxs-lookup"><span data-stu-id="9f616-131">Name of the tab.</span></span>     |
|  <span data-ttu-id="9f616-132">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="9f616-132">sortOrderIndex</span></span>  |   <span data-ttu-id="9f616-133">整数</span><span class="sxs-lookup"><span data-stu-id="9f616-133">int</span></span>                     |  <span data-ttu-id="9f616-134">用于排序选项卡的顺序的索引</span><span class="sxs-lookup"><span data-stu-id="9f616-134">Index of the order used for sorting tabs</span></span>     |
|  <span data-ttu-id="9f616-135">webUrl</span><span class="sxs-lookup"><span data-stu-id="9f616-135">webUrl</span></span>          |   <span data-ttu-id="9f616-136">string</span><span class="sxs-lookup"><span data-stu-id="9f616-136">string</span></span>                  |  <span data-ttu-id="9f616-137">深度链接的选项卡实例的 url。</span><span class="sxs-lookup"><span data-stu-id="9f616-137">Deep link url of the tab instance.</span></span> <span data-ttu-id="9f616-138">只读。</span><span class="sxs-lookup"><span data-stu-id="9f616-138">Read only.</span></span>     |
|  <span data-ttu-id="9f616-139">configuration</span><span class="sxs-lookup"><span data-stu-id="9f616-139">configuration</span></span>        |   [<span data-ttu-id="9f616-140">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="9f616-140">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="9f616-141">应用于选项卡的自定义设置的容器。配置仅后设置此属性时，才视为选项卡。</span><span class="sxs-lookup"><span data-stu-id="9f616-141">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="9f616-142">Relationships</span><span class="sxs-lookup"><span data-stu-id="9f616-142">Relationships</span></span>

| <span data-ttu-id="9f616-143">关系</span><span class="sxs-lookup"><span data-stu-id="9f616-143">Relationship</span></span> | <span data-ttu-id="9f616-144">类型</span><span class="sxs-lookup"><span data-stu-id="9f616-144">Type</span></span>   | <span data-ttu-id="9f616-145">说明</span><span class="sxs-lookup"><span data-stu-id="9f616-145">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9f616-146">teamsApp</span><span class="sxs-lookup"><span data-stu-id="9f616-146">teamsApp</span></span>|[<span data-ttu-id="9f616-147">teamsApp</span><span class="sxs-lookup"><span data-stu-id="9f616-147">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="9f616-148">应用程序的链接到选项卡。这不能更改选项卡创建后。</span><span class="sxs-lookup"><span data-stu-id="9f616-148">The application that is linked to the tab. This cannot be changed after tab creation.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9f616-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9f616-149">JSON representation</span></span>

<span data-ttu-id="9f616-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f616-150">The following is a JSON representation of the resource.</span></span>


<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.teamsTab"
}-->

```json
{  
  "id": "string",
  "displayName": "string",
  "sortOrderIndex": "string",
  "webUrl": "string",
  "configuration" : "teamsTabConfiguration"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsTab resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="9f616-151">另请参阅</span><span class="sxs-lookup"><span data-stu-id="9f616-151">See also</span></span>

[<span data-ttu-id="9f616-152">配置到内置选项卡的类型</span><span class="sxs-lookup"><span data-stu-id="9f616-152">Configuring the built-in tab types</span></span>](../../../concepts/teams-configuring-builtin-tabs.md)
