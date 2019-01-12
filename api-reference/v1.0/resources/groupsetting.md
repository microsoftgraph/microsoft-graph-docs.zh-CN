---
title: groupSetting 资源类型
description: 组设置控制行为，如组显示名称的禁止使用的词语列表，或是否允许来宾用户成为组所有者。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 42e6c0dc0f0ffd48da84023c5e4ff0d97cb446f2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911691"
---
# <a name="groupsetting-resource-type"></a><span data-ttu-id="68b81-103">groupSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="68b81-103">groupSetting resource type</span></span>

<span data-ttu-id="68b81-104">组设置控制行为，如组显示名称的禁止使用的词语列表，或是否允许来宾用户成为组所有者。</span><span class="sxs-lookup"><span data-stu-id="68b81-104">Group settings control behaviors such as blocked word lists for group display names or whether guest users are allowed to be group owners.</span></span>

<span data-ttu-id="68b81-p101">组设置可根据可用的 [groupSettingTemplates](groupsettingtemplate.md) 进行创建，并可更改其预设默认值。这些设置在租户范围级别或特定组内控制组行为。当在租户范围和特定组中定义相同的设置时，组级设置将替代租户范围的设置。例如，租户范围的设置可能允许现有组成员邀请来宾，但是单独组设置可以替代此操作，并且不允许组成员邀请来宾。组设置只控制 Office 365 组行为。</span><span class="sxs-lookup"><span data-stu-id="68b81-p101">Group settings can be created based on the available [groupSettingTemplates](groupsettingtemplate.md), and changed from their preset defaults. These settings govern group behaviors at a tenant-wide level or to a specific group. When the same setting is defined at both the tenant-wide and to a specific group, the group-level setting overrides the tenant-wide setting.  For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but an individual group setting can override and not allow guests to be invited by members of the group. Group settings only govern Office 365 groups behavior.</span></span>

## <a name="methods"></a><span data-ttu-id="68b81-110">方法</span><span class="sxs-lookup"><span data-stu-id="68b81-110">Methods</span></span>

| <span data-ttu-id="68b81-111">方法</span><span class="sxs-lookup"><span data-stu-id="68b81-111">Method</span></span> | <span data-ttu-id="68b81-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="68b81-112">Return Type</span></span> | <span data-ttu-id="68b81-113">说明</span><span class="sxs-lookup"><span data-stu-id="68b81-113">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="68b81-114">创建设置</span><span class="sxs-lookup"><span data-stu-id="68b81-114">Create setting</span></span>](../api/groupsetting-post-groupsettings.md) | [<span data-ttu-id="68b81-115">groupSetting</span><span class="sxs-lookup"><span data-stu-id="68b81-115">groupSetting</span></span>](groupsetting.md) |<span data-ttu-id="68b81-p102">基于 groupSettingTemplate 创建设置对象。POST 请求必须为模板中定义的所有设置提供 settingValues。</span><span class="sxs-lookup"><span data-stu-id="68b81-p102">Create a setting object based on a groupSettingTemplate. The POST request must provide settingValues for all the settings defined in the template.</span></span> |
|[<span data-ttu-id="68b81-118">获取设置</span><span class="sxs-lookup"><span data-stu-id="68b81-118">Get setting</span></span>](../api/groupsetting-get.md) | [<span data-ttu-id="68b81-119">groupSetting</span><span class="sxs-lookup"><span data-stu-id="68b81-119">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="68b81-120">读取特定设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="68b81-120">Read properties of a specific setting object.</span></span> |
|[<span data-ttu-id="68b81-121">列出设置</span><span class="sxs-lookup"><span data-stu-id="68b81-121">List settings</span></span>](../api/groupsetting-list.md) | <span data-ttu-id="68b81-122">[groupSetting](groupsetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="68b81-122">[groupSetting](groupsetting.md) collection</span></span> | <span data-ttu-id="68b81-123">列出所有设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="68b81-123">List properties of all setting objects.</span></span> |
|[<span data-ttu-id="68b81-124">更新设置</span><span class="sxs-lookup"><span data-stu-id="68b81-124">Update setting</span></span>](../api/groupsetting-update.md) | [<span data-ttu-id="68b81-125">groupSetting</span><span class="sxs-lookup"><span data-stu-id="68b81-125">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="68b81-126">更新 groupsetting 对象。</span><span class="sxs-lookup"><span data-stu-id="68b81-126">Update groupsetting object.</span></span> |
|[<span data-ttu-id="68b81-127">删除设置</span><span class="sxs-lookup"><span data-stu-id="68b81-127">Delete setting</span></span>](../api/groupsetting-delete.md) | <span data-ttu-id="68b81-128">无</span><span class="sxs-lookup"><span data-stu-id="68b81-128">None</span></span> | <span data-ttu-id="68b81-129">删除设置对象。</span><span class="sxs-lookup"><span data-stu-id="68b81-129">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="68b81-130">属性</span><span class="sxs-lookup"><span data-stu-id="68b81-130">Properties</span></span>

| <span data-ttu-id="68b81-131">属性</span><span class="sxs-lookup"><span data-stu-id="68b81-131">Property</span></span> | <span data-ttu-id="68b81-132">类型</span><span class="sxs-lookup"><span data-stu-id="68b81-132">Type</span></span> | <span data-ttu-id="68b81-133">说明</span><span class="sxs-lookup"><span data-stu-id="68b81-133">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="68b81-134">displayName</span><span class="sxs-lookup"><span data-stu-id="68b81-134">displayName</span></span>|<span data-ttu-id="68b81-135">字符串</span><span class="sxs-lookup"><span data-stu-id="68b81-135">String</span></span>| <span data-ttu-id="68b81-136">来自相关模板的此组设置的显示名称。</span><span class="sxs-lookup"><span data-stu-id="68b81-136">Display name of this group of settings, which comes from the associated template.</span></span> |
|<span data-ttu-id="68b81-137">id</span><span class="sxs-lookup"><span data-stu-id="68b81-137">id</span></span>|<span data-ttu-id="68b81-138">字符串</span><span class="sxs-lookup"><span data-stu-id="68b81-138">String</span></span>| <span data-ttu-id="68b81-p103">这些设置的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="68b81-p103">Unique identifier for these settings. Read-only.</span></span> |
|<span data-ttu-id="68b81-141">templateId</span><span class="sxs-lookup"><span data-stu-id="68b81-141">templateId</span></span>|<span data-ttu-id="68b81-142">字符串</span><span class="sxs-lookup"><span data-stu-id="68b81-142">String</span></span>| <span data-ttu-id="68b81-p104">用于创建此组设置的模板的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="68b81-p104">Unique identifier for the template used to create this group of settings. Read-only.</span></span> |
|<span data-ttu-id="68b81-145">values</span><span class="sxs-lookup"><span data-stu-id="68b81-145">values</span></span>|<span data-ttu-id="68b81-146">[settingValue](settingvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="68b81-146">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="68b81-p105">名称值对的集合。必须包含并设置模板中定义的所有设置。</span><span class="sxs-lookup"><span data-stu-id="68b81-p105">Collection of name value pairs. Must contain and set all the settings defined in the template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="68b81-149">关系</span><span class="sxs-lookup"><span data-stu-id="68b81-149">Relationships</span></span>

<span data-ttu-id="68b81-150">无。</span><span class="sxs-lookup"><span data-stu-id="68b81-150">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="68b81-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="68b81-151">JSON representation</span></span>

<span data-ttu-id="68b81-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="68b81-152">Here is a JSON representation of the resource.</span></span>

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
