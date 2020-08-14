---
title: groupSetting 资源类型
description: 组设置控制诸如组显示名称阻止的单词列表的行为，或者是否允许来宾用户成为组所有者。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 8c20ecd7452477519e5543dfd36a02aa5796cd38
ms.sourcegitcommit: 5c3f4a3e2620d1d9e635e09231bbaa73cb0c3cdd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/14/2020
ms.locfileid: "46674067"
---
# <a name="groupsetting-resource-type"></a><span data-ttu-id="4f394-103">groupSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="4f394-103">groupSetting resource type</span></span>

<span data-ttu-id="4f394-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f394-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4f394-105">组设置控制诸如组显示名称阻止的单词列表的行为，或者是否允许来宾用户成为组所有者。</span><span class="sxs-lookup"><span data-stu-id="4f394-105">Group settings control behaviors such as blocked word lists for group display names or whether guest users are allowed to be group owners.</span></span>

<span data-ttu-id="4f394-106">可以基于可用的 [groupSettingTemplates](groupsettingtemplate.md)创建组设置，并将其从预设默认值更改为。</span><span class="sxs-lookup"><span data-stu-id="4f394-106">Group settings can be created based on the available [groupSettingTemplates](groupsettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="4f394-107">这些设置管理租户级或特定组的组行为。</span><span class="sxs-lookup"><span data-stu-id="4f394-107">These settings govern group behaviors at a tenant-wide level or to a specific group.</span></span> <span data-ttu-id="4f394-108">当同时在租户范围和特定组中定义相同设置时，组级别设置将覆盖租户范围内的设置。</span><span class="sxs-lookup"><span data-stu-id="4f394-108">When the same setting is defined at both the tenant-wide and to a specific group, the group-level setting overrides the tenant-wide setting.</span></span>  <span data-ttu-id="4f394-109">例如，租户范围内的设置可能会允许来宾受到现有组成员的邀请，但单个组设置可以覆盖，而不允许由组成员邀请来宾。</span><span class="sxs-lookup"><span data-stu-id="4f394-109">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but an individual group setting can override and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="4f394-110">组设置仅控制 Microsoft 365 组的行为。</span><span class="sxs-lookup"><span data-stu-id="4f394-110">Group settings only govern Microsoft 365 groups behavior.</span></span>

## <a name="methods"></a><span data-ttu-id="4f394-111">方法</span><span class="sxs-lookup"><span data-stu-id="4f394-111">Methods</span></span>

| <span data-ttu-id="4f394-112">方法</span><span class="sxs-lookup"><span data-stu-id="4f394-112">Method</span></span> | <span data-ttu-id="4f394-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="4f394-113">Return Type</span></span> | <span data-ttu-id="4f394-114">说明</span><span class="sxs-lookup"><span data-stu-id="4f394-114">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="4f394-115">Create setting</span><span class="sxs-lookup"><span data-stu-id="4f394-115">Create setting</span></span>](../api/groupsetting-post-groupsettings.md) | [<span data-ttu-id="4f394-116">groupSetting</span><span class="sxs-lookup"><span data-stu-id="4f394-116">groupSetting</span></span>](groupsetting.md) |<span data-ttu-id="4f394-117">创建基于 groupSettingTemplate 的 setting 对象。</span><span class="sxs-lookup"><span data-stu-id="4f394-117">Create a setting object based on a groupSettingTemplate.</span></span> <span data-ttu-id="4f394-118">POST 请求必须为模板中定义的所有设置提供 settingValues。</span><span class="sxs-lookup"><span data-stu-id="4f394-118">The POST request must provide settingValues for all the settings defined in the template.</span></span> |
|[<span data-ttu-id="4f394-119">获取设置</span><span class="sxs-lookup"><span data-stu-id="4f394-119">Get setting</span></span>](../api/groupsetting-get.md) | [<span data-ttu-id="4f394-120">groupSetting</span><span class="sxs-lookup"><span data-stu-id="4f394-120">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="4f394-121">读取特定设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4f394-121">Read properties of a specific setting object.</span></span> |
|[<span data-ttu-id="4f394-122">列出设置</span><span class="sxs-lookup"><span data-stu-id="4f394-122">List settings</span></span>](../api/groupsetting-list.md) | <span data-ttu-id="4f394-123">[groupSetting](groupsetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4f394-123">[groupSetting](groupsetting.md) collection</span></span> | <span data-ttu-id="4f394-124">列出所有设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4f394-124">List properties of all setting objects.</span></span> |
|[<span data-ttu-id="4f394-125">更新设置</span><span class="sxs-lookup"><span data-stu-id="4f394-125">Update setting</span></span>](../api/groupsetting-update.md) | [<span data-ttu-id="4f394-126">groupSetting</span><span class="sxs-lookup"><span data-stu-id="4f394-126">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="4f394-127">更新 groupsetting 对象。</span><span class="sxs-lookup"><span data-stu-id="4f394-127">Update groupsetting object.</span></span> |
|[<span data-ttu-id="4f394-128">删除设置</span><span class="sxs-lookup"><span data-stu-id="4f394-128">Delete setting</span></span>](../api/groupsetting-delete.md) | <span data-ttu-id="4f394-129">无</span><span class="sxs-lookup"><span data-stu-id="4f394-129">None</span></span> | <span data-ttu-id="4f394-130">删除 setting 对象。</span><span class="sxs-lookup"><span data-stu-id="4f394-130">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4f394-131">属性</span><span class="sxs-lookup"><span data-stu-id="4f394-131">Properties</span></span>

| <span data-ttu-id="4f394-132">属性</span><span class="sxs-lookup"><span data-stu-id="4f394-132">Property</span></span> | <span data-ttu-id="4f394-133">类型</span><span class="sxs-lookup"><span data-stu-id="4f394-133">Type</span></span> | <span data-ttu-id="4f394-134">说明</span><span class="sxs-lookup"><span data-stu-id="4f394-134">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="4f394-135">displayName</span><span class="sxs-lookup"><span data-stu-id="4f394-135">displayName</span></span>|<span data-ttu-id="4f394-136">String</span><span class="sxs-lookup"><span data-stu-id="4f394-136">String</span></span>| <span data-ttu-id="4f394-137">来自关联模板的此组设置的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4f394-137">Display name of this group of settings, which comes from the associated template.</span></span> |
|<span data-ttu-id="4f394-138">id</span><span class="sxs-lookup"><span data-stu-id="4f394-138">id</span></span>|<span data-ttu-id="4f394-139">String</span><span class="sxs-lookup"><span data-stu-id="4f394-139">String</span></span>| <span data-ttu-id="4f394-140">这些设置的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4f394-140">Unique identifier for these settings.</span></span> <span data-ttu-id="4f394-141">只读。</span><span class="sxs-lookup"><span data-stu-id="4f394-141">Read-only.</span></span> |
|<span data-ttu-id="4f394-142">templateId</span><span class="sxs-lookup"><span data-stu-id="4f394-142">templateId</span></span>|<span data-ttu-id="4f394-143">String</span><span class="sxs-lookup"><span data-stu-id="4f394-143">String</span></span>| <span data-ttu-id="4f394-144">用于创建此组设置的模板的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4f394-144">Unique identifier for the template used to create this group of settings.</span></span> <span data-ttu-id="4f394-145">只读。</span><span class="sxs-lookup"><span data-stu-id="4f394-145">Read-only.</span></span> |
|<span data-ttu-id="4f394-146">values</span><span class="sxs-lookup"><span data-stu-id="4f394-146">values</span></span>|<span data-ttu-id="4f394-147">[settingValue](settingvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4f394-147">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="4f394-148">名称值对的集合。</span><span class="sxs-lookup"><span data-stu-id="4f394-148">Collection of name value pairs.</span></span> <span data-ttu-id="4f394-149">必须包含并设置在模板中定义的所有设置。</span><span class="sxs-lookup"><span data-stu-id="4f394-149">Must contain and set all the settings defined in the template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="4f394-150">关系</span><span class="sxs-lookup"><span data-stu-id="4f394-150">Relationships</span></span>

<span data-ttu-id="4f394-151">无。</span><span class="sxs-lookup"><span data-stu-id="4f394-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f394-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4f394-152">JSON representation</span></span>

<span data-ttu-id="4f394-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f394-153">Here is a JSON representation of the resource.</span></span>

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
