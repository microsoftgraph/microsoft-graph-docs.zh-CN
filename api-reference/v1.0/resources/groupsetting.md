# <a name="groupsetting-resource-type"></a><span data-ttu-id="53837-101">groupSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="53837-101">groupSetting resource type</span></span>

<span data-ttu-id="53837-102">组设置控制行为，如组显示名称的禁止使用的词语列表，或是否允许来宾用户成为组所有者。</span><span class="sxs-lookup"><span data-stu-id="53837-102">Group settings control behaviors such as blocked word lists for group display names or whether guest users are allowed to be group owners.</span></span>

<span data-ttu-id="53837-p101">组设置可根据可用的 [groupSettingTemplates](groupSettingTemplate.md) 进行创建，并可更改其预设默认值。这些设置在租户范围级别或特定组内控制组行为。当在租户范围和特定组中定义相同的设置时，组级设置将替代租户范围的设置。例如，租户范围的设置可能允许现有组成员邀请来宾，但是单独组设置可以替代此操作，并且不允许组成员邀请来宾。组设置只控制 Office 365 组行为。</span><span class="sxs-lookup"><span data-stu-id="53837-p101">Group settings can be created based on the available [groupSettingTemplates](groupSettingTemplate.md), and changed from their preset defaults. These settings govern group behaviors at a tenant-wide level or to a specific group. When the same setting is defined at both the tenant-wide and to a specific group, the group-level setting overrides the tenant-wide setting.  For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but an individual group setting can override and not allow guests to be invited by members of the group. Group settings only govern Office 365 groups behavior.</span></span>

## <a name="methods"></a><span data-ttu-id="53837-108">方法</span><span class="sxs-lookup"><span data-stu-id="53837-108">Methods</span></span>

| <span data-ttu-id="53837-109">方法</span><span class="sxs-lookup"><span data-stu-id="53837-109">Method</span></span> | <span data-ttu-id="53837-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="53837-110">Return Type</span></span> | <span data-ttu-id="53837-111">说明</span><span class="sxs-lookup"><span data-stu-id="53837-111">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="53837-112">创建设置</span><span class="sxs-lookup"><span data-stu-id="53837-112">Create setting</span></span>](../api/groupsetting_post_groupsettings.md) | [<span data-ttu-id="53837-113">groupSetting</span><span class="sxs-lookup"><span data-stu-id="53837-113">groupSetting</span></span>](groupsetting.md) |<span data-ttu-id="53837-p102">基于 groupSettingTemplate 创建设置对象。POST 请求必须为模板中定义的所有设置提供 settingValues。</span><span class="sxs-lookup"><span data-stu-id="53837-p102">Create a setting object based on a groupSettingTemplate. The POST request must provide settingValues for all the settings defined in the template.</span></span> |
|[<span data-ttu-id="53837-116">获取设置</span><span class="sxs-lookup"><span data-stu-id="53837-116">Get setting</span></span>](../api/groupsetting_get.md) | [<span data-ttu-id="53837-117">groupSetting</span><span class="sxs-lookup"><span data-stu-id="53837-117">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="53837-118">读取特定设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="53837-118">Read properties of a specific setting object.</span></span> |
|[<span data-ttu-id="53837-119">列出设置</span><span class="sxs-lookup"><span data-stu-id="53837-119">List settings</span></span>](../api/groupsetting_list.md) | <span data-ttu-id="53837-120">[groupSetting](groupsetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="53837-120">[groupSetting](groupsetting.md) collection</span></span> | <span data-ttu-id="53837-121">列出所有设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="53837-121">List properties of all setting objects.</span></span> |
|[<span data-ttu-id="53837-122">更新设置</span><span class="sxs-lookup"><span data-stu-id="53837-122">Update setting</span></span>](../api/groupsetting_update.md) | [<span data-ttu-id="53837-123">groupSetting</span><span class="sxs-lookup"><span data-stu-id="53837-123">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="53837-124">更新 groupsetting 对象。</span><span class="sxs-lookup"><span data-stu-id="53837-124">Update groupsetting object.</span></span> |
|[<span data-ttu-id="53837-125">删除设置</span><span class="sxs-lookup"><span data-stu-id="53837-125">Delete setting</span></span>](../api/groupsetting_delete.md) | <span data-ttu-id="53837-126">无</span><span class="sxs-lookup"><span data-stu-id="53837-126">None</span></span> | <span data-ttu-id="53837-127">删除设置对象。</span><span class="sxs-lookup"><span data-stu-id="53837-127">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="53837-128">属性</span><span class="sxs-lookup"><span data-stu-id="53837-128">Properties</span></span>

| <span data-ttu-id="53837-129">属性</span><span class="sxs-lookup"><span data-stu-id="53837-129">Property</span></span> | <span data-ttu-id="53837-130">类型</span><span class="sxs-lookup"><span data-stu-id="53837-130">Type</span></span> | <span data-ttu-id="53837-131">说明</span><span class="sxs-lookup"><span data-stu-id="53837-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="53837-132">displayName</span><span class="sxs-lookup"><span data-stu-id="53837-132">displayName</span></span>|<span data-ttu-id="53837-133">字符串</span><span class="sxs-lookup"><span data-stu-id="53837-133">String</span></span>| <span data-ttu-id="53837-134">来自相关模板的此组设置的显示名称。</span><span class="sxs-lookup"><span data-stu-id="53837-134">Display name of this group of settings, which comes from the associated template.</span></span> |
|<span data-ttu-id="53837-135">id</span><span class="sxs-lookup"><span data-stu-id="53837-135">id</span></span>|<span data-ttu-id="53837-136">字符串</span><span class="sxs-lookup"><span data-stu-id="53837-136">String</span></span>| <span data-ttu-id="53837-p103">这些设置的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="53837-p103">Unique identifier for these settings. Read-only.</span></span> |
|<span data-ttu-id="53837-139">templateId</span><span class="sxs-lookup"><span data-stu-id="53837-139">templateId</span></span>|<span data-ttu-id="53837-140">字符串</span><span class="sxs-lookup"><span data-stu-id="53837-140">String</span></span>| <span data-ttu-id="53837-p104">用于创建此组设置的模板的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="53837-p104">Unique identifier for the template used to create this group of settings. Read-only.</span></span> |
|<span data-ttu-id="53837-143">values</span><span class="sxs-lookup"><span data-stu-id="53837-143">values</span></span>|<span data-ttu-id="53837-144">[settingValue](settingvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="53837-144">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="53837-p105">名称值对的集合。必须包含并设置模板中定义的所有设置。</span><span class="sxs-lookup"><span data-stu-id="53837-p105">Collection of name value pairs. Must contain and set all the settings defined in the template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="53837-147">关系</span><span class="sxs-lookup"><span data-stu-id="53837-147">Relationships</span></span>

<span data-ttu-id="53837-148">无。</span><span class="sxs-lookup"><span data-stu-id="53837-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="53837-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="53837-149">JSON representation</span></span>

<span data-ttu-id="53837-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53837-150">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.groupSetting"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "templateId": "String",
  "values": [{"@odata.type": "microsoft.graph.settingValue"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->