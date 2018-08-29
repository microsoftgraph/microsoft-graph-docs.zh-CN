# <a name="groupsettingtemplate-resource-type"></a><span data-ttu-id="66488-101">groupSettingTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="66488-101">groupSettingTemplate resource type</span></span>

<span data-ttu-id="66488-p101">组设置模板表示租户可用的系统定义设置。[组设置](groupsetting.md)可根据可用的 **groupSettingTemplates** 和从其预设默认值更改的值进行创建。无法创建、更新或删除组设置模板。这些设置可以表示租户范围设置，也可以表示特定组设置。目前，唯一可用的模板可应用于 Office 365 组，并且包括诸如用户是否可以创建组或邀请来自组织外的来宾成为组成员的设置。</span><span class="sxs-lookup"><span data-stu-id="66488-p101">Group setting templates represent system-defined settings available to the tenant. [Group settings](groupsetting.md) can be created based on the available **groupSettingTemplates**, and values changed from their preset defaults. Group setting templates cannot be created, updated or deleted. These settings can represent tenant-wide settings, or can represent specific group settings. Currently, the only templates available apply to Office 365 groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

## <a name="methods"></a><span data-ttu-id="66488-107">方法</span><span class="sxs-lookup"><span data-stu-id="66488-107">Methods</span></span>

| <span data-ttu-id="66488-108">方法</span><span class="sxs-lookup"><span data-stu-id="66488-108">Method</span></span> | <span data-ttu-id="66488-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="66488-109">Return Type</span></span> | <span data-ttu-id="66488-110">说明</span><span class="sxs-lookup"><span data-stu-id="66488-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="66488-111">Get groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="66488-111">Get groupSettingTemplate</span></span>](../api/groupsettingtemplate_get.md) | [<span data-ttu-id="66488-112">groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="66488-112">groupSettingTemplate</span></span>](groupsettingtemplate.md) | <span data-ttu-id="66488-113">读取其中一个系统定义的 groupSettingTemplate 对象的特定属性。</span><span class="sxs-lookup"><span data-stu-id="66488-113">Read the specific properties of one of the system defined groupSettingTemplate objects.</span></span> |
|[<span data-ttu-id="66488-114">List groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="66488-114">List groupSettingTemplate</span></span>](../api/groupsettingtemplate_list.md) | [<span data-ttu-id="66488-115">groupSettingTemplate 集合</span><span class="sxs-lookup"><span data-stu-id="66488-115">Collection of groupSettingTemplate</span></span>](groupsettingtemplate.md) |<span data-ttu-id="66488-116">列出所有系统定义的 groupSettingTemplate 对象。</span><span class="sxs-lookup"><span data-stu-id="66488-116">List all of the system defined groupSettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="66488-117">属性</span><span class="sxs-lookup"><span data-stu-id="66488-117">Properties</span></span>

| <span data-ttu-id="66488-118">属性</span><span class="sxs-lookup"><span data-stu-id="66488-118">Property</span></span> | <span data-ttu-id="66488-119">类型</span><span class="sxs-lookup"><span data-stu-id="66488-119">Type</span></span> | <span data-ttu-id="66488-120">说明</span><span class="sxs-lookup"><span data-stu-id="66488-120">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="66488-121">说明</span><span class="sxs-lookup"><span data-stu-id="66488-121">description</span></span>|<span data-ttu-id="66488-122">字符串</span><span class="sxs-lookup"><span data-stu-id="66488-122">String</span></span>| <span data-ttu-id="66488-123">模板描述</span><span class="sxs-lookup"><span data-stu-id="66488-123">Description of the template.</span></span> |
|<span data-ttu-id="66488-124">displayName</span><span class="sxs-lookup"><span data-stu-id="66488-124">displayName</span></span>|<span data-ttu-id="66488-125">字符串</span><span class="sxs-lookup"><span data-stu-id="66488-125">String</span></span>| <span data-ttu-id="66488-126">模板的显示名称</span><span class="sxs-lookup"><span data-stu-id="66488-126">Display name of the template.</span></span> |
|<span data-ttu-id="66488-127">id</span><span class="sxs-lookup"><span data-stu-id="66488-127">id</span></span>|<span data-ttu-id="66488-128">字符串</span><span class="sxs-lookup"><span data-stu-id="66488-128">String</span></span>| <span data-ttu-id="66488-p102">模板的的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="66488-p102">Unique identifier for the template. Read-only.</span></span>|
|<span data-ttu-id="66488-131">values</span><span class="sxs-lookup"><span data-stu-id="66488-131">values</span></span>|<span data-ttu-id="66488-132">[settingTemplateValue](settingtemplatevalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="66488-132">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="66488-133">setTemplateValues 的集合，列出组成此模板的一组可用设置、默认值和类型。</span><span class="sxs-lookup"><span data-stu-id="66488-133">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="66488-134">关系</span><span class="sxs-lookup"><span data-stu-id="66488-134">Relationships</span></span>

<span data-ttu-id="66488-135">无。</span><span class="sxs-lookup"><span data-stu-id="66488-135">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="66488-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="66488-136">JSON representation</span></span>

<span data-ttu-id="66488-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66488-137">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.groupSettingTemplate"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "values": [{"@odata.type": "microsoft.graph.settingTemplateValue"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupSettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->