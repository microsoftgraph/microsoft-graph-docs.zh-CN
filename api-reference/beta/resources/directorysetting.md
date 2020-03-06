---
title: directorySetting 资源类型
description: 可以基于可用的 directorySettingTemplates 创建目录设置，并将其更改为预设的默认值。 这些设置可以控制实体或功能行为，既可以在租户范围级别，也可以在特定实体级别进行。 如果在租户范围和特定实体级别定义相同的设置，则特定实体级别设置可能会从租户范围设置中退出。  例如，租户范围内的设置可能会允许来宾受到现有组成员的邀请，但特定的组设置可能会退出，而不允许由组成员邀请来宾。 当前的系统定义的设置仅控制 Office 组的行为。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1d42e46d39e28357d6839111a5e6a865b421cf87
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42506629"
---
# <a name="directorysetting-resource-type"></a><span data-ttu-id="7291f-107">directorySetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="7291f-107">directorySetting resource type</span></span>

<span data-ttu-id="7291f-108">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7291f-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7291f-109">可以基于可用的[directorySettingTemplates](directorysettingtemplate.md)创建目录设置，并将其更改为预设的默认值。</span><span class="sxs-lookup"><span data-stu-id="7291f-109">Directory settings can be created based on the available [directorySettingTemplates](directorysettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="7291f-110">这些设置可以控制实体或功能行为，既可以在租户范围级别，也可以在特定实体级别进行。</span><span class="sxs-lookup"><span data-stu-id="7291f-110">These settings can govern entity or feature behaviors, both at a tenant-wide level or at a specific entity level.</span></span> <span data-ttu-id="7291f-111">如果在租户范围和特定实体级别定义相同的设置，则特定实体级别设置可能会从租户范围设置中退出。</span><span class="sxs-lookup"><span data-stu-id="7291f-111">When the same setting is defined at both the tenant-wide and specific entity level, the specific entity level setting may opt-out from the tenant-wide setting.</span></span>  <span data-ttu-id="7291f-112">例如，租户范围内的设置可能会允许来宾受到现有组成员的邀请，但特定的组设置可能会退出，而不允许由组成员邀请来宾。</span><span class="sxs-lookup"><span data-stu-id="7291f-112">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but a specific group setting may opt-out and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="7291f-113">当前的系统定义的设置仅控制 Office 组的行为。</span><span class="sxs-lookup"><span data-stu-id="7291f-113">Currently system defined settings are only govern Office groups behavior.</span></span>

> <span data-ttu-id="7291f-114">**注意**： directorySetting 资源类型的/beta 版本仅适用于组。</span><span class="sxs-lookup"><span data-stu-id="7291f-114">**Note**: The /beta version of the directorySetting resource type only applies to groups.</span></span> <span data-ttu-id="7291f-115">/V1.0 版本已重命名为 groupSetting。</span><span class="sxs-lookup"><span data-stu-id="7291f-115">The /v1.0 version has been renamed to groupSetting.</span></span>

## <a name="methods"></a><span data-ttu-id="7291f-116">Methods</span><span class="sxs-lookup"><span data-stu-id="7291f-116">Methods</span></span>

| <span data-ttu-id="7291f-117">方法</span><span class="sxs-lookup"><span data-stu-id="7291f-117">Method</span></span>           | <span data-ttu-id="7291f-118">返回类型</span><span class="sxs-lookup"><span data-stu-id="7291f-118">Return Type</span></span>    |<span data-ttu-id="7291f-119">说明</span><span class="sxs-lookup"><span data-stu-id="7291f-119">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7291f-120">Create setting</span><span class="sxs-lookup"><span data-stu-id="7291f-120">Create setting</span></span>](../api/directorysetting-post-settings.md) | [<span data-ttu-id="7291f-121">directorySetting</span><span class="sxs-lookup"><span data-stu-id="7291f-121">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="7291f-122">创建基于 directorySettingTemplate 的 setting 对象。</span><span class="sxs-lookup"><span data-stu-id="7291f-122">Create a setting object based on a directorySettingTemplate.</span></span> <span data-ttu-id="7291f-123">POST 请求必须为模板中定义的所有设置提供 settingValues。</span><span class="sxs-lookup"><span data-stu-id="7291f-123">The POST request must provide settingValues for all the settings defined in the template.</span></span>|
|[<span data-ttu-id="7291f-124">Get setting</span><span class="sxs-lookup"><span data-stu-id="7291f-124">Get setting</span></span>](../api/directorysetting-get.md) | [<span data-ttu-id="7291f-125">directorySetting</span><span class="sxs-lookup"><span data-stu-id="7291f-125">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="7291f-126">读取特定设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7291f-126">Read properties of a specific setting object.</span></span>|
|[<span data-ttu-id="7291f-127">List settings</span><span class="sxs-lookup"><span data-stu-id="7291f-127">List settings</span></span>](../api/directorysetting-list.md) | <span data-ttu-id="7291f-128">[directorySetting](directorysetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7291f-128">[directorySetting](directorysetting.md) collection</span></span> |<span data-ttu-id="7291f-129">列出所有设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7291f-129">List properties of all setting objects.</span></span>|
|[<span data-ttu-id="7291f-130">Update setting</span><span class="sxs-lookup"><span data-stu-id="7291f-130">Update setting</span></span>](../api/directorysetting-update.md) | [<span data-ttu-id="7291f-131">directorySetting</span><span class="sxs-lookup"><span data-stu-id="7291f-131">directorySetting</span></span>](directorysetting.md)  |<span data-ttu-id="7291f-132">更新 setting 对象。</span><span class="sxs-lookup"><span data-stu-id="7291f-132">Update a setting object.</span></span> <span data-ttu-id="7291f-133">仅在更新中可以更改 settingValues。</span><span class="sxs-lookup"><span data-stu-id="7291f-133">Only settingValues can be changed in an update.</span></span>|
|[<span data-ttu-id="7291f-134">删除设置</span><span class="sxs-lookup"><span data-stu-id="7291f-134">Delete setting</span></span>](../api/directorysetting-delete.md) | <span data-ttu-id="7291f-135">无</span><span class="sxs-lookup"><span data-stu-id="7291f-135">None</span></span> |<span data-ttu-id="7291f-136">删除 setting 对象。</span><span class="sxs-lookup"><span data-stu-id="7291f-136">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7291f-137">属性</span><span class="sxs-lookup"><span data-stu-id="7291f-137">Properties</span></span>
| <span data-ttu-id="7291f-138">属性</span><span class="sxs-lookup"><span data-stu-id="7291f-138">Property</span></span>     | <span data-ttu-id="7291f-139">类型</span><span class="sxs-lookup"><span data-stu-id="7291f-139">Type</span></span>   |<span data-ttu-id="7291f-140">说明</span><span class="sxs-lookup"><span data-stu-id="7291f-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7291f-141">displayName</span><span class="sxs-lookup"><span data-stu-id="7291f-141">displayName</span></span>|<span data-ttu-id="7291f-142">string</span><span class="sxs-lookup"><span data-stu-id="7291f-142">string</span></span>|<span data-ttu-id="7291f-143">来自关联模板的此组设置的显示名称。</span><span class="sxs-lookup"><span data-stu-id="7291f-143">Display name of this group of settings, which comes from the associated template.</span></span> <span data-ttu-id="7291f-144">只读。</span><span class="sxs-lookup"><span data-stu-id="7291f-144">Read-only.</span></span>|
|<span data-ttu-id="7291f-145">id</span><span class="sxs-lookup"><span data-stu-id="7291f-145">id</span></span>|<span data-ttu-id="7291f-146">string</span><span class="sxs-lookup"><span data-stu-id="7291f-146">string</span></span>| <span data-ttu-id="7291f-147">这些设置的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="7291f-147">Unique identifier for these settings.</span></span> <span data-ttu-id="7291f-148">只读。</span><span class="sxs-lookup"><span data-stu-id="7291f-148">Read-only.</span></span>|
|<span data-ttu-id="7291f-149">templateId</span><span class="sxs-lookup"><span data-stu-id="7291f-149">templateId</span></span>|<span data-ttu-id="7291f-150">字符串</span><span class="sxs-lookup"><span data-stu-id="7291f-150">string</span></span>| <span data-ttu-id="7291f-151">用于创建此组设置的模板的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="7291f-151">Unique identifier for the template used to create this group of settings.</span></span> <span data-ttu-id="7291f-152">只读。</span><span class="sxs-lookup"><span data-stu-id="7291f-152">Read-only.</span></span>|
|<span data-ttu-id="7291f-153">values</span><span class="sxs-lookup"><span data-stu-id="7291f-153">values</span></span>|<span data-ttu-id="7291f-154">[settingValue](settingvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="7291f-154">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="7291f-155">名称值对的集合。</span><span class="sxs-lookup"><span data-stu-id="7291f-155">Collection of name value pairs.</span></span> <span data-ttu-id="7291f-156">必须包含并设置在模板中定义的所有设置。</span><span class="sxs-lookup"><span data-stu-id="7291f-156">Must contain and set all the settings defined in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7291f-157">关系</span><span class="sxs-lookup"><span data-stu-id="7291f-157">Relationships</span></span>
<span data-ttu-id="7291f-158">无</span><span class="sxs-lookup"><span data-stu-id="7291f-158">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="7291f-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7291f-159">JSON representation</span></span>

<span data-ttu-id="7291f-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7291f-160">Here is a JSON representation of the resource.</span></span>

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
