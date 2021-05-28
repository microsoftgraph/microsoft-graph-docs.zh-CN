---
title: groupSetting 资源类型
description: 组设置控制行为，如阻止组显示名称的单词列表或是否允许来宾用户成为组所有者。
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 1e18f78f0b0d7c9e8cb9c054afd5645ae45e1c48
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680876"
---
# <a name="groupsetting-resource-type"></a><span data-ttu-id="faceb-103">groupSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="faceb-103">groupSetting resource type</span></span>

<span data-ttu-id="faceb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="faceb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="faceb-105">组设置控制行为，如阻止组显示名称的单词列表或是否允许来宾用户成为组所有者。</span><span class="sxs-lookup"><span data-stu-id="faceb-105">Group settings control behaviors such as blocked word lists for group display names or whether guest users are allowed to be group owners.</span></span>

<span data-ttu-id="faceb-106">可以基于可用的 [groupSettingTemplates](groupsettingtemplate.md)创建组设置，并更改其预设默认值。</span><span class="sxs-lookup"><span data-stu-id="faceb-106">Group settings can be created based on the available [groupSettingTemplates](groupsettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="faceb-107">这些设置控制租户范围内或特定组的组行为。</span><span class="sxs-lookup"><span data-stu-id="faceb-107">These settings govern group behaviors at a tenant-wide level or to a specific group.</span></span> <span data-ttu-id="faceb-108">当在租户范围和特定组上定义相同设置时，组级别设置将覆盖租户范围的设置。</span><span class="sxs-lookup"><span data-stu-id="faceb-108">When the same setting is defined at both the tenant-wide and to a specific group, the group-level setting overrides the tenant-wide setting.</span></span>  <span data-ttu-id="faceb-109">例如，租户范围设置可能允许现有组成员邀请来宾，但单个组设置可以覆盖并不允许组的成员邀请来宾。</span><span class="sxs-lookup"><span data-stu-id="faceb-109">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but an individual group setting can override and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="faceb-110">组设置仅控制Microsoft 365组行为。</span><span class="sxs-lookup"><span data-stu-id="faceb-110">Group settings only govern Microsoft 365 groups behavior.</span></span>

## <a name="methods"></a><span data-ttu-id="faceb-111">方法</span><span class="sxs-lookup"><span data-stu-id="faceb-111">Methods</span></span>

| <span data-ttu-id="faceb-112">方法</span><span class="sxs-lookup"><span data-stu-id="faceb-112">Method</span></span> | <span data-ttu-id="faceb-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="faceb-113">Return Type</span></span> | <span data-ttu-id="faceb-114">说明</span><span class="sxs-lookup"><span data-stu-id="faceb-114">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="faceb-115">Create setting</span><span class="sxs-lookup"><span data-stu-id="faceb-115">Create setting</span></span>](../api/groupsetting-post-groupsettings.md) | [<span data-ttu-id="faceb-116">groupSetting</span><span class="sxs-lookup"><span data-stu-id="faceb-116">groupSetting</span></span>](groupsetting.md) |<span data-ttu-id="faceb-117">创建基于 groupSettingTemplate 的设置对象。</span><span class="sxs-lookup"><span data-stu-id="faceb-117">Create a setting object based on a groupSettingTemplate.</span></span> <span data-ttu-id="faceb-118">POST 请求必须为模板中定义的所有设置提供 settingValues。</span><span class="sxs-lookup"><span data-stu-id="faceb-118">The POST request must provide settingValues for all the settings defined in the template.</span></span> |
|[<span data-ttu-id="faceb-119">获取设置</span><span class="sxs-lookup"><span data-stu-id="faceb-119">Get setting</span></span>](../api/groupsetting-get.md) | [<span data-ttu-id="faceb-120">groupSetting</span><span class="sxs-lookup"><span data-stu-id="faceb-120">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="faceb-121">读取特定设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="faceb-121">Read properties of a specific setting object.</span></span> |
|[<span data-ttu-id="faceb-122">List settings</span><span class="sxs-lookup"><span data-stu-id="faceb-122">List settings</span></span>](../api/groupsetting-list.md) | <span data-ttu-id="faceb-123">[groupSetting](groupsetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="faceb-123">[groupSetting](groupsetting.md) collection</span></span> | <span data-ttu-id="faceb-124">列出所有设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="faceb-124">List properties of all setting objects.</span></span> |
|[<span data-ttu-id="faceb-125">更新设置</span><span class="sxs-lookup"><span data-stu-id="faceb-125">Update setting</span></span>](../api/groupsetting-update.md) | [<span data-ttu-id="faceb-126">groupSetting</span><span class="sxs-lookup"><span data-stu-id="faceb-126">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="faceb-127">更新 groupsetting 对象。</span><span class="sxs-lookup"><span data-stu-id="faceb-127">Update groupsetting object.</span></span> |
|[<span data-ttu-id="faceb-128">删除设置</span><span class="sxs-lookup"><span data-stu-id="faceb-128">Delete setting</span></span>](../api/groupsetting-delete.md) | <span data-ttu-id="faceb-129">无</span><span class="sxs-lookup"><span data-stu-id="faceb-129">None</span></span> | <span data-ttu-id="faceb-130">删除 setting 对象。</span><span class="sxs-lookup"><span data-stu-id="faceb-130">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="faceb-131">属性</span><span class="sxs-lookup"><span data-stu-id="faceb-131">Properties</span></span>

| <span data-ttu-id="faceb-132">属性</span><span class="sxs-lookup"><span data-stu-id="faceb-132">Property</span></span> | <span data-ttu-id="faceb-133">类型</span><span class="sxs-lookup"><span data-stu-id="faceb-133">Type</span></span> | <span data-ttu-id="faceb-134">说明</span><span class="sxs-lookup"><span data-stu-id="faceb-134">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="faceb-135">displayName</span><span class="sxs-lookup"><span data-stu-id="faceb-135">displayName</span></span>|<span data-ttu-id="faceb-136">String</span><span class="sxs-lookup"><span data-stu-id="faceb-136">String</span></span>| <span data-ttu-id="faceb-137">这组设置的显示名称，来自关联的模板。</span><span class="sxs-lookup"><span data-stu-id="faceb-137">Display name of this group of settings, which comes from the associated template.</span></span> |
|<span data-ttu-id="faceb-138">id</span><span class="sxs-lookup"><span data-stu-id="faceb-138">id</span></span>|<span data-ttu-id="faceb-139">String</span><span class="sxs-lookup"><span data-stu-id="faceb-139">String</span></span>| <span data-ttu-id="faceb-140">这些设置的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="faceb-140">Unique identifier for these settings.</span></span> <span data-ttu-id="faceb-141">只读。</span><span class="sxs-lookup"><span data-stu-id="faceb-141">Read-only.</span></span> |
|<span data-ttu-id="faceb-142">templateId</span><span class="sxs-lookup"><span data-stu-id="faceb-142">templateId</span></span>|<span data-ttu-id="faceb-143">String</span><span class="sxs-lookup"><span data-stu-id="faceb-143">String</span></span>| <span data-ttu-id="faceb-144">用于创建这组设置的模板的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="faceb-144">Unique identifier for the template used to create this group of settings.</span></span> <span data-ttu-id="faceb-145">只读。</span><span class="sxs-lookup"><span data-stu-id="faceb-145">Read-only.</span></span> |
|<span data-ttu-id="faceb-146">values</span><span class="sxs-lookup"><span data-stu-id="faceb-146">values</span></span>|<span data-ttu-id="faceb-147">[settingValue](settingvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="faceb-147">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="faceb-148">名称值对的集合。</span><span class="sxs-lookup"><span data-stu-id="faceb-148">Collection of name value pairs.</span></span> <span data-ttu-id="faceb-149">必须包含和设置模板中定义的所有设置。</span><span class="sxs-lookup"><span data-stu-id="faceb-149">Must contain and set all the settings defined in the template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="faceb-150">关系</span><span class="sxs-lookup"><span data-stu-id="faceb-150">Relationships</span></span>

<span data-ttu-id="faceb-151">无。</span><span class="sxs-lookup"><span data-stu-id="faceb-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="faceb-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="faceb-152">JSON representation</span></span>

<span data-ttu-id="faceb-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="faceb-153">Here is a JSON representation of the resource.</span></span>

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

