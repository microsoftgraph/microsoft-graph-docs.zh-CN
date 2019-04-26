---
title: groupSetting 资源类型
description: 组设置控制诸如组显示名称阻止的单词列表的行为, 或者是否允许来宾用户成为组所有者。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 42e6c0dc0f0ffd48da84023c5e4ff0d97cb446f2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570825"
---
# <a name="groupsetting-resource-type"></a><span data-ttu-id="0e458-103">groupSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="0e458-103">groupSetting resource type</span></span>

<span data-ttu-id="0e458-104">组设置控制诸如组显示名称阻止的单词列表的行为, 或者是否允许来宾用户成为组所有者。</span><span class="sxs-lookup"><span data-stu-id="0e458-104">Group settings control behaviors such as blocked word lists for group display names or whether guest users are allowed to be group owners.</span></span>

<span data-ttu-id="0e458-105">可以基于可用的[groupSettingTemplates](groupsettingtemplate.md)创建组设置, 并将其从预设默认值更改为。</span><span class="sxs-lookup"><span data-stu-id="0e458-105">Group settings can be created based on the available [groupSettingTemplates](groupsettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="0e458-106">这些设置管理租户级或特定组的组行为。</span><span class="sxs-lookup"><span data-stu-id="0e458-106">These settings govern group behaviors at a tenant-wide level or to a specific group.</span></span> <span data-ttu-id="0e458-107">当同时在租户范围和特定组中定义相同设置时, 组级别设置将覆盖租户范围内的设置。</span><span class="sxs-lookup"><span data-stu-id="0e458-107">When the same setting is defined at both the tenant-wide and to a specific group, the group-level setting overrides the tenant-wide setting.</span></span>  <span data-ttu-id="0e458-108">例如, 租户范围内的设置可能会允许来宾受到现有组成员的邀请, 但单个组设置可以覆盖, 而不允许由组成员邀请来宾。</span><span class="sxs-lookup"><span data-stu-id="0e458-108">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but an individual group setting can override and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="0e458-109">组设置仅控制 Office 365 组的行为。</span><span class="sxs-lookup"><span data-stu-id="0e458-109">Group settings only govern Office 365 groups behavior.</span></span>

## <a name="methods"></a><span data-ttu-id="0e458-110">方法</span><span class="sxs-lookup"><span data-stu-id="0e458-110">Methods</span></span>

| <span data-ttu-id="0e458-111">方法</span><span class="sxs-lookup"><span data-stu-id="0e458-111">Method</span></span> | <span data-ttu-id="0e458-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="0e458-112">Return Type</span></span> | <span data-ttu-id="0e458-113">说明</span><span class="sxs-lookup"><span data-stu-id="0e458-113">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="0e458-114">创建设置</span><span class="sxs-lookup"><span data-stu-id="0e458-114">Create setting</span></span>](../api/groupsetting-post-groupsettings.md) | [<span data-ttu-id="0e458-115">groupSetting</span><span class="sxs-lookup"><span data-stu-id="0e458-115">groupSetting</span></span>](groupsetting.md) |<span data-ttu-id="0e458-116">创建基于 groupSettingTemplate 的 setting 对象。</span><span class="sxs-lookup"><span data-stu-id="0e458-116">Create a setting object based on a groupSettingTemplate.</span></span> <span data-ttu-id="0e458-117">POST 请求必须为模板中定义的所有设置提供 settingValues。</span><span class="sxs-lookup"><span data-stu-id="0e458-117">The POST request must provide settingValues for all the settings defined in the template.</span></span> |
|[<span data-ttu-id="0e458-118">获取设置</span><span class="sxs-lookup"><span data-stu-id="0e458-118">Get setting</span></span>](../api/groupsetting-get.md) | [<span data-ttu-id="0e458-119">groupSetting</span><span class="sxs-lookup"><span data-stu-id="0e458-119">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="0e458-120">读取特定设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0e458-120">Read properties of a specific setting object.</span></span> |
|[<span data-ttu-id="0e458-121">列出设置</span><span class="sxs-lookup"><span data-stu-id="0e458-121">List settings</span></span>](../api/groupsetting-list.md) | <span data-ttu-id="0e458-122">[groupSetting](groupsetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0e458-122">[groupSetting](groupsetting.md) collection</span></span> | <span data-ttu-id="0e458-123">列出所有设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0e458-123">List properties of all setting objects.</span></span> |
|[<span data-ttu-id="0e458-124">更新设置</span><span class="sxs-lookup"><span data-stu-id="0e458-124">Update setting</span></span>](../api/groupsetting-update.md) | [<span data-ttu-id="0e458-125">groupSetting</span><span class="sxs-lookup"><span data-stu-id="0e458-125">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="0e458-126">更新 groupsetting 对象。</span><span class="sxs-lookup"><span data-stu-id="0e458-126">Update groupsetting object.</span></span> |
|[<span data-ttu-id="0e458-127">删除设置</span><span class="sxs-lookup"><span data-stu-id="0e458-127">Delete setting</span></span>](../api/groupsetting-delete.md) | <span data-ttu-id="0e458-128">无</span><span class="sxs-lookup"><span data-stu-id="0e458-128">None</span></span> | <span data-ttu-id="0e458-129">删除 setting 对象。</span><span class="sxs-lookup"><span data-stu-id="0e458-129">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0e458-130">属性</span><span class="sxs-lookup"><span data-stu-id="0e458-130">Properties</span></span>

| <span data-ttu-id="0e458-131">属性</span><span class="sxs-lookup"><span data-stu-id="0e458-131">Property</span></span> | <span data-ttu-id="0e458-132">类型</span><span class="sxs-lookup"><span data-stu-id="0e458-132">Type</span></span> | <span data-ttu-id="0e458-133">说明</span><span class="sxs-lookup"><span data-stu-id="0e458-133">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0e458-134">displayName</span><span class="sxs-lookup"><span data-stu-id="0e458-134">displayName</span></span>|<span data-ttu-id="0e458-135">String</span><span class="sxs-lookup"><span data-stu-id="0e458-135">String</span></span>| <span data-ttu-id="0e458-136">来自关联模板的此组设置的显示名称。</span><span class="sxs-lookup"><span data-stu-id="0e458-136">Display name of this group of settings, which comes from the associated template.</span></span> |
|<span data-ttu-id="0e458-137">id</span><span class="sxs-lookup"><span data-stu-id="0e458-137">id</span></span>|<span data-ttu-id="0e458-138">String</span><span class="sxs-lookup"><span data-stu-id="0e458-138">String</span></span>| <span data-ttu-id="0e458-139">这些设置的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0e458-139">Unique identifier for these settings.</span></span> <span data-ttu-id="0e458-140">只读。</span><span class="sxs-lookup"><span data-stu-id="0e458-140">Read-only.</span></span> |
|<span data-ttu-id="0e458-141">templateId</span><span class="sxs-lookup"><span data-stu-id="0e458-141">templateId</span></span>|<span data-ttu-id="0e458-142">String</span><span class="sxs-lookup"><span data-stu-id="0e458-142">String</span></span>| <span data-ttu-id="0e458-143">用于创建此组设置的模板的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0e458-143">Unique identifier for the template used to create this group of settings.</span></span> <span data-ttu-id="0e458-144">只读。</span><span class="sxs-lookup"><span data-stu-id="0e458-144">Read-only.</span></span> |
|<span data-ttu-id="0e458-145">值</span><span class="sxs-lookup"><span data-stu-id="0e458-145">values</span></span>|<span data-ttu-id="0e458-146">[settingValue](settingvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="0e458-146">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="0e458-147">名称值对的集合。</span><span class="sxs-lookup"><span data-stu-id="0e458-147">Collection of name value pairs.</span></span> <span data-ttu-id="0e458-148">必须包含并设置在模板中定义的所有设置。</span><span class="sxs-lookup"><span data-stu-id="0e458-148">Must contain and set all the settings defined in the template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0e458-149">关系</span><span class="sxs-lookup"><span data-stu-id="0e458-149">Relationships</span></span>

<span data-ttu-id="0e458-150">无。</span><span class="sxs-lookup"><span data-stu-id="0e458-150">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e458-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0e458-151">JSON representation</span></span>

<span data-ttu-id="0e458-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e458-152">Here is a JSON representation of the resource.</span></span>

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
