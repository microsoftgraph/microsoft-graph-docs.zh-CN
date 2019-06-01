---
title: directorySetting 资源类型
description: 可以基于可用的 directorySettingTemplates 创建目录设置, 并将其更改为预设的默认值。 这些设置可以控制实体或功能行为, 既可以在租户范围级别, 也可以在特定实体级别进行。 如果在租户范围和特定实体级别定义相同的设置, 则特定实体级别设置可能会从租户范围设置中退出。  例如, 租户范围内的设置可能会允许来宾受到现有组成员的邀请, 但特定的组设置可能会退出, 而不允许由组成员邀请来宾。 当前的系统定义的设置仅控制 Office 组的行为。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3eccdb3b19acb286a8b67393f9a7b441b108627c
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657880"
---
# <a name="directorysetting-resource-type"></a><span data-ttu-id="9c571-107">directorySetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="9c571-107">directorySetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c571-108">可以基于可用的[directorySettingTemplates](directorysettingtemplate.md)创建目录设置, 并将其更改为预设的默认值。</span><span class="sxs-lookup"><span data-stu-id="9c571-108">Directory settings can be created based on the available [directorySettingTemplates](directorysettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="9c571-109">这些设置可以控制实体或功能行为, 既可以在租户范围级别, 也可以在特定实体级别进行。</span><span class="sxs-lookup"><span data-stu-id="9c571-109">These settings can govern entity or feature behaviors, both at a tenant-wide level or at a specific entity level.</span></span> <span data-ttu-id="9c571-110">如果在租户范围和特定实体级别定义相同的设置, 则特定实体级别设置可能会从租户范围设置中退出。</span><span class="sxs-lookup"><span data-stu-id="9c571-110">When the same setting is defined at both the tenant-wide and specific entity level, the specific entity level setting may opt-out from the tenant-wide setting.</span></span>  <span data-ttu-id="9c571-111">例如, 租户范围内的设置可能会允许来宾受到现有组成员的邀请, 但特定的组设置可能会退出, 而不允许由组成员邀请来宾。</span><span class="sxs-lookup"><span data-stu-id="9c571-111">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but a specific group setting may opt-out and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="9c571-112">当前的系统定义的设置仅控制 Office 组的行为。</span><span class="sxs-lookup"><span data-stu-id="9c571-112">Currently system defined settings are only govern Office groups behavior.</span></span>

> <span data-ttu-id="9c571-113">**注意**: directorySetting 资源类型的/beta 版本仅适用于组。</span><span class="sxs-lookup"><span data-stu-id="9c571-113">**Note**: The /beta version of the directorySetting resource type only applies to groups.</span></span> <span data-ttu-id="9c571-114">/V1.0 版本已重命名为 groupSetting。</span><span class="sxs-lookup"><span data-stu-id="9c571-114">The /v1.0 version has been renamed to groupSetting.</span></span>

## <a name="methods"></a><span data-ttu-id="9c571-115">方法</span><span class="sxs-lookup"><span data-stu-id="9c571-115">Methods</span></span>

| <span data-ttu-id="9c571-116">方法</span><span class="sxs-lookup"><span data-stu-id="9c571-116">Method</span></span>           | <span data-ttu-id="9c571-117">返回类型</span><span class="sxs-lookup"><span data-stu-id="9c571-117">Return Type</span></span>    |<span data-ttu-id="9c571-118">说明</span><span class="sxs-lookup"><span data-stu-id="9c571-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9c571-119">Create setting</span><span class="sxs-lookup"><span data-stu-id="9c571-119">Create setting</span></span>](../api/directorysetting-post-settings.md) | [<span data-ttu-id="9c571-120">directorySetting</span><span class="sxs-lookup"><span data-stu-id="9c571-120">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="9c571-121">创建基于 directorySettingTemplate 的 setting 对象。</span><span class="sxs-lookup"><span data-stu-id="9c571-121">Create a setting object based on a directorySettingTemplate.</span></span> <span data-ttu-id="9c571-122">POST 请求必须为模板中定义的所有设置提供 settingValues。</span><span class="sxs-lookup"><span data-stu-id="9c571-122">The POST request must provide settingValues for all the settings defined in the template.</span></span>|
|[<span data-ttu-id="9c571-123">Get setting</span><span class="sxs-lookup"><span data-stu-id="9c571-123">Get setting</span></span>](../api/directorysetting-get.md) | [<span data-ttu-id="9c571-124">directorySetting</span><span class="sxs-lookup"><span data-stu-id="9c571-124">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="9c571-125">读取特定设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9c571-125">Read properties of a specific setting object.</span></span>|
|[<span data-ttu-id="9c571-126">List settings</span><span class="sxs-lookup"><span data-stu-id="9c571-126">List settings</span></span>](../api/directorysetting-list.md) | <span data-ttu-id="9c571-127">[directorySetting](directorysetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9c571-127">[directorySetting](directorysetting.md) collection</span></span> |<span data-ttu-id="9c571-128">列出所有设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9c571-128">List properties of all setting objects.</span></span>|
|[<span data-ttu-id="9c571-129">Update setting</span><span class="sxs-lookup"><span data-stu-id="9c571-129">Update setting</span></span>](../api/directorysetting-update.md) | [<span data-ttu-id="9c571-130">directorySetting</span><span class="sxs-lookup"><span data-stu-id="9c571-130">directorySetting</span></span>](directorysetting.md)  |<span data-ttu-id="9c571-131">更新 setting 对象。</span><span class="sxs-lookup"><span data-stu-id="9c571-131">Update a setting object.</span></span> <span data-ttu-id="9c571-132">仅在更新中可以更改 settingValues。</span><span class="sxs-lookup"><span data-stu-id="9c571-132">Only settingValues can be changed in an update.</span></span>|
|[<span data-ttu-id="9c571-133">删除设置</span><span class="sxs-lookup"><span data-stu-id="9c571-133">Delete setting</span></span>](../api/directorysetting-delete.md) | <span data-ttu-id="9c571-134">无</span><span class="sxs-lookup"><span data-stu-id="9c571-134">None</span></span> |<span data-ttu-id="9c571-135">删除 setting 对象。</span><span class="sxs-lookup"><span data-stu-id="9c571-135">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9c571-136">属性</span><span class="sxs-lookup"><span data-stu-id="9c571-136">Properties</span></span>
| <span data-ttu-id="9c571-137">属性</span><span class="sxs-lookup"><span data-stu-id="9c571-137">Property</span></span>     | <span data-ttu-id="9c571-138">类型</span><span class="sxs-lookup"><span data-stu-id="9c571-138">Type</span></span>   |<span data-ttu-id="9c571-139">说明</span><span class="sxs-lookup"><span data-stu-id="9c571-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c571-140">displayName</span><span class="sxs-lookup"><span data-stu-id="9c571-140">displayName</span></span>|<span data-ttu-id="9c571-141">string</span><span class="sxs-lookup"><span data-stu-id="9c571-141">string</span></span>|<span data-ttu-id="9c571-142">来自关联模板的此组设置的显示名称。</span><span class="sxs-lookup"><span data-stu-id="9c571-142">Display name of this group of settings, which comes from the associated template.</span></span> <span data-ttu-id="9c571-143">只读。</span><span class="sxs-lookup"><span data-stu-id="9c571-143">Read-only.</span></span>|
|<span data-ttu-id="9c571-144">id</span><span class="sxs-lookup"><span data-stu-id="9c571-144">id</span></span>|<span data-ttu-id="9c571-145">string</span><span class="sxs-lookup"><span data-stu-id="9c571-145">string</span></span>| <span data-ttu-id="9c571-146">这些设置的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9c571-146">Unique identifier for these settings.</span></span> <span data-ttu-id="9c571-147">只读。</span><span class="sxs-lookup"><span data-stu-id="9c571-147">Read-only.</span></span>|
|<span data-ttu-id="9c571-148">templateId</span><span class="sxs-lookup"><span data-stu-id="9c571-148">templateId</span></span>|<span data-ttu-id="9c571-149">字符串</span><span class="sxs-lookup"><span data-stu-id="9c571-149">string</span></span>| <span data-ttu-id="9c571-150">用于创建此组设置的模板的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9c571-150">Unique identifier for the template used to create this group of settings.</span></span> <span data-ttu-id="9c571-151">只读。</span><span class="sxs-lookup"><span data-stu-id="9c571-151">Read-only.</span></span>|
|<span data-ttu-id="9c571-152">values</span><span class="sxs-lookup"><span data-stu-id="9c571-152">values</span></span>|<span data-ttu-id="9c571-153">[settingValue](settingvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="9c571-153">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="9c571-154">名称值对的集合。</span><span class="sxs-lookup"><span data-stu-id="9c571-154">Collection of name value pairs.</span></span> <span data-ttu-id="9c571-155">必须包含并设置在模板中定义的所有设置。</span><span class="sxs-lookup"><span data-stu-id="9c571-155">Must contain and set all the settings defined in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c571-156">关系</span><span class="sxs-lookup"><span data-stu-id="9c571-156">Relationships</span></span>
<span data-ttu-id="9c571-157">无</span><span class="sxs-lookup"><span data-stu-id="9c571-157">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9c571-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9c571-158">JSON representation</span></span>

<span data-ttu-id="9c571-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9c571-159">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySetting"
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "templateId": "string",
  "values": [{"@odata.type": "microsoft.graph.settingValue"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directorySetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
