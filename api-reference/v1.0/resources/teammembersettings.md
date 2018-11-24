# <a name="teammembersettings-resource-type"></a><span data-ttu-id="3e7d2-101">teamMemberSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="3e7d2-101">teamMemberSettings resource type</span></span>



<span data-ttu-id="3e7d2-102">例如，要配置的成员可以执行某些操作时，是否设置创建通道，并将自动程序，添加[团队](team.md)中。</span><span class="sxs-lookup"><span data-stu-id="3e7d2-102">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3e7d2-103">属性</span><span class="sxs-lookup"><span data-stu-id="3e7d2-103">Properties</span></span>
| <span data-ttu-id="3e7d2-104">属性</span><span class="sxs-lookup"><span data-stu-id="3e7d2-104">Property</span></span>     | <span data-ttu-id="3e7d2-105">类型</span><span class="sxs-lookup"><span data-stu-id="3e7d2-105">Type</span></span>   |<span data-ttu-id="3e7d2-106">说明</span><span class="sxs-lookup"><span data-stu-id="3e7d2-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e7d2-107">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="3e7d2-107">allowCreateUpdateChannels</span></span>|<span data-ttu-id="3e7d2-108">布尔</span><span class="sxs-lookup"><span data-stu-id="3e7d2-108">Boolean</span></span>|<span data-ttu-id="3e7d2-109">如果设置为 true，则成员可以添加和更新通道。</span><span class="sxs-lookup"><span data-stu-id="3e7d2-109">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="3e7d2-110">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="3e7d2-110">allowDeleteChannels</span></span>|<span data-ttu-id="3e7d2-111">布尔</span><span class="sxs-lookup"><span data-stu-id="3e7d2-111">Boolean</span></span>|<span data-ttu-id="3e7d2-112">如果设置为 true，则成员可以删除通道。</span><span class="sxs-lookup"><span data-stu-id="3e7d2-112">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="3e7d2-113">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="3e7d2-113">allowAddRemoveApps</span></span>|<span data-ttu-id="3e7d2-114">布尔</span><span class="sxs-lookup"><span data-stu-id="3e7d2-114">Boolean</span></span>|<span data-ttu-id="3e7d2-115">如果设置为 true，则成员可以添加和删除应用程序。</span><span class="sxs-lookup"><span data-stu-id="3e7d2-115">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="3e7d2-116">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="3e7d2-116">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="3e7d2-117">布尔</span><span class="sxs-lookup"><span data-stu-id="3e7d2-117">Boolean</span></span>|<span data-ttu-id="3e7d2-118">如果设置为 true，则成员可以添加、 更新和删除选项卡。</span><span class="sxs-lookup"><span data-stu-id="3e7d2-118">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="3e7d2-119">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="3e7d2-119">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="3e7d2-120">布尔</span><span class="sxs-lookup"><span data-stu-id="3e7d2-120">Boolean</span></span>|<span data-ttu-id="3e7d2-121">如果设置为 true，则成员可以添加、 更新和删除连接器。</span><span class="sxs-lookup"><span data-stu-id="3e7d2-121">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3e7d2-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e7d2-122">JSON representation</span></span>

<span data-ttu-id="3e7d2-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e7d2-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMemberSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true,
  "allowAddRemoveApps": true,
  "allowCreateUpdateRemoveTabs": true,
  "allowCreateUpdateRemoveConnectors": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's memberSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
