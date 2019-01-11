---
title: groupSettingTemplate 资源类型
description: 组设置模板表示租户可用的系统定义设置。组设置可根据可用的 **groupSettingTemplates** 和从其预设默认值更改的值进行创建。无法创建、更新或删除组设置模板。这些设置可以表示租户范围设置，也可以表示特定组设置。目前，唯一可用的模板可应用于 Office 365 组，并且包括诸如用户是否可以创建组或邀请来自组织外的来宾成为组成员的设置。
localization_priority: Normal
ms.openlocfilehash: c2e6b465226b8c1c69438fab37d874735e89ac52
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859344"
---
# <a name="groupsettingtemplate-resource-type"></a><span data-ttu-id="0638b-107">groupSettingTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="0638b-107">groupSettingTemplate resource type</span></span>

<span data-ttu-id="0638b-p102">组设置模板表示租户可用的系统定义设置。[组设置](groupsetting.md)可根据可用的 **groupSettingTemplates** 和从其预设默认值更改的值进行创建。无法创建、更新或删除组设置模板。这些设置可以表示租户范围设置，也可以表示特定组设置。目前，唯一可用的模板可应用于 Office 365 组，并且包括诸如用户是否可以创建组或邀请来自组织外的来宾成为组成员的设置。</span><span class="sxs-lookup"><span data-stu-id="0638b-p102">Group setting templates represent system-defined settings available to the tenant. [Group settings](groupsetting.md) can be created based on the available **groupSettingTemplates**, and values changed from their preset defaults. Group setting templates cannot be created, updated or deleted. These settings can represent tenant-wide settings, or can represent specific group settings. Currently, the only templates available apply to Office 365 groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

## <a name="methods"></a><span data-ttu-id="0638b-113">方法</span><span class="sxs-lookup"><span data-stu-id="0638b-113">Methods</span></span>

| <span data-ttu-id="0638b-114">方法</span><span class="sxs-lookup"><span data-stu-id="0638b-114">Method</span></span> | <span data-ttu-id="0638b-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="0638b-115">Return Type</span></span> | <span data-ttu-id="0638b-116">说明</span><span class="sxs-lookup"><span data-stu-id="0638b-116">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="0638b-117">Get groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="0638b-117">Get groupSettingTemplate</span></span>](../api/groupsettingtemplate-get.md) | [<span data-ttu-id="0638b-118">groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="0638b-118">groupSettingTemplate</span></span>](groupsettingtemplate.md) | <span data-ttu-id="0638b-119">读取其中一个系统定义的 groupSettingTemplate 对象的特定属性。</span><span class="sxs-lookup"><span data-stu-id="0638b-119">Read the specific properties of one of the system defined groupSettingTemplate objects.</span></span> |
|[<span data-ttu-id="0638b-120">List groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="0638b-120">List groupSettingTemplate</span></span>](../api/groupsettingtemplate-list.md) | [<span data-ttu-id="0638b-121">groupSettingTemplate 集合</span><span class="sxs-lookup"><span data-stu-id="0638b-121">Collection of groupSettingTemplate</span></span>](groupsettingtemplate.md) |<span data-ttu-id="0638b-122">列出所有系统定义的 groupSettingTemplate 对象。</span><span class="sxs-lookup"><span data-stu-id="0638b-122">List all of the system defined groupSettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="0638b-123">属性</span><span class="sxs-lookup"><span data-stu-id="0638b-123">Properties</span></span>

| <span data-ttu-id="0638b-124">属性</span><span class="sxs-lookup"><span data-stu-id="0638b-124">Property</span></span> | <span data-ttu-id="0638b-125">类型</span><span class="sxs-lookup"><span data-stu-id="0638b-125">Type</span></span> | <span data-ttu-id="0638b-126">说明</span><span class="sxs-lookup"><span data-stu-id="0638b-126">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0638b-127">说明</span><span class="sxs-lookup"><span data-stu-id="0638b-127">description</span></span>|<span data-ttu-id="0638b-128">字符串</span><span class="sxs-lookup"><span data-stu-id="0638b-128">String</span></span>| <span data-ttu-id="0638b-129">模板描述</span><span class="sxs-lookup"><span data-stu-id="0638b-129">Description of the template.</span></span> |
|<span data-ttu-id="0638b-130">displayName</span><span class="sxs-lookup"><span data-stu-id="0638b-130">displayName</span></span>|<span data-ttu-id="0638b-131">字符串</span><span class="sxs-lookup"><span data-stu-id="0638b-131">String</span></span>| <span data-ttu-id="0638b-132">模板的显示名称</span><span class="sxs-lookup"><span data-stu-id="0638b-132">Display name of the template.</span></span> |
|<span data-ttu-id="0638b-133">id</span><span class="sxs-lookup"><span data-stu-id="0638b-133">id</span></span>|<span data-ttu-id="0638b-134">字符串</span><span class="sxs-lookup"><span data-stu-id="0638b-134">String</span></span>| <span data-ttu-id="0638b-p103">模板的的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="0638b-p103">Unique identifier for the template. Read-only.</span></span>|
|<span data-ttu-id="0638b-137">values</span><span class="sxs-lookup"><span data-stu-id="0638b-137">values</span></span>|<span data-ttu-id="0638b-138">[settingTemplateValue](settingtemplatevalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0638b-138">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="0638b-139">setTemplateValues 的集合，列出组成此模板的一组可用设置、默认值和类型。</span><span class="sxs-lookup"><span data-stu-id="0638b-139">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0638b-140">关系</span><span class="sxs-lookup"><span data-stu-id="0638b-140">Relationships</span></span>

<span data-ttu-id="0638b-141">无。</span><span class="sxs-lookup"><span data-stu-id="0638b-141">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="0638b-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0638b-142">JSON representation</span></span>

<span data-ttu-id="0638b-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0638b-143">Here is a JSON representation of the resource.</span></span>

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
