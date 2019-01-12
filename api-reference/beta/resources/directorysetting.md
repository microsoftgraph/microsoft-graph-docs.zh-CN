---
title: directorySetting 资源类型
description: 可以创建基于可用 directorySettingTemplates，并从其预设的默认值更改目录设置。 这些设置可以控制实体或功能行为，同时在租户范围级别或特定实体级别。 在租户范围和特定实体级别定义相同的设置后，特定实体级别设置可能会选择退出从租户范围的设置。  例如，租户范围的设置可能允许来宾要邀请的现有组的成员，但的特定组设置可能会选择退出，并且不允许来宾要邀请的组的成员。 当前定义的系统设置是仅控制 Office 组行为。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fbe1879a22b2dc7e69258d34f7e25c37bfd0cd5a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990549"
---
# <a name="directorysetting-resource-type"></a><span data-ttu-id="9601f-107">directorySetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="9601f-107">directorySetting resource type</span></span>

> <span data-ttu-id="9601f-108">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9601f-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9601f-109">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9601f-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9601f-110">可以创建基于可用[directorySettingTemplates](directorysettingtemplate.md)，并从其预设的默认值更改目录设置。</span><span class="sxs-lookup"><span data-stu-id="9601f-110">Directory settings can be created based on the available [directorySettingTemplates](directorysettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="9601f-111">这些设置可以控制实体或功能行为，同时在租户范围级别或特定实体级别。</span><span class="sxs-lookup"><span data-stu-id="9601f-111">These settings can govern entity or feature behaviors, both at a tenant-wide level or at a specific entity level.</span></span> <span data-ttu-id="9601f-112">在租户范围和特定实体级别定义相同的设置后，特定实体级别设置可能会选择退出从租户范围的设置。</span><span class="sxs-lookup"><span data-stu-id="9601f-112">When the same setting is defined at both the tenant-wide and specific entity level, the specific entity level setting may opt-out from the tenant-wide setting.</span></span>  <span data-ttu-id="9601f-113">例如，租户范围的设置可能允许来宾要邀请的现有组的成员，但的特定组设置可能会选择退出，并且不允许来宾要邀请的组的成员。</span><span class="sxs-lookup"><span data-stu-id="9601f-113">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but a specific group setting may opt-out and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="9601f-114">当前定义的系统设置是仅控制 Office 组行为。</span><span class="sxs-lookup"><span data-stu-id="9601f-114">Currently system defined settings are only govern Office groups behavior.</span></span>

> <span data-ttu-id="9601f-115">**注意**： directorySetting 资源类型的 /beta 版本仅适用于组。</span><span class="sxs-lookup"><span data-stu-id="9601f-115">**Note**: The /beta version of the directorySetting resource type only applies to groups.</span></span> <span data-ttu-id="9601f-116">/V1.0 版本已被重命名为 groupSetting。</span><span class="sxs-lookup"><span data-stu-id="9601f-116">The /v1.0 version has been renamed to groupSetting.</span></span>

## <a name="methods"></a><span data-ttu-id="9601f-117">方法</span><span class="sxs-lookup"><span data-stu-id="9601f-117">Methods</span></span>

| <span data-ttu-id="9601f-118">方法</span><span class="sxs-lookup"><span data-stu-id="9601f-118">Method</span></span>           | <span data-ttu-id="9601f-119">返回类型</span><span class="sxs-lookup"><span data-stu-id="9601f-119">Return Type</span></span>    |<span data-ttu-id="9601f-120">说明</span><span class="sxs-lookup"><span data-stu-id="9601f-120">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9601f-121">创建设置</span><span class="sxs-lookup"><span data-stu-id="9601f-121">Create setting</span></span>](../api/directorysetting-post-settings.md) | [<span data-ttu-id="9601f-122">directorySetting</span><span class="sxs-lookup"><span data-stu-id="9601f-122">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="9601f-123">创建基于 directorySettingTemplate 设置对象。</span><span class="sxs-lookup"><span data-stu-id="9601f-123">Create a setting object based on a directorySettingTemplate.</span></span> <span data-ttu-id="9601f-124">POST 请求必须提供 settingValues 模板中定义的所有设置。</span><span class="sxs-lookup"><span data-stu-id="9601f-124">The POST request must provide settingValues for all the settings defined in the template.</span></span>|
|[<span data-ttu-id="9601f-125">获取设置</span><span class="sxs-lookup"><span data-stu-id="9601f-125">Get setting</span></span>](../api/directorysetting-get.md) | [<span data-ttu-id="9601f-126">directorySetting</span><span class="sxs-lookup"><span data-stu-id="9601f-126">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="9601f-127">读取特定设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9601f-127">Read properties of a specific setting object.</span></span>|
|[<span data-ttu-id="9601f-128">列出设置</span><span class="sxs-lookup"><span data-stu-id="9601f-128">List settings</span></span>](../api/directorysetting-list.md) | <span data-ttu-id="9601f-129">[directorySetting](directorysetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="9601f-129">[directorySetting](directorysetting.md) collection</span></span> |<span data-ttu-id="9601f-130">列出所有设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9601f-130">List properties of all setting objects.</span></span>|
|[<span data-ttu-id="9601f-131">更新设置</span><span class="sxs-lookup"><span data-stu-id="9601f-131">Update setting</span></span>](../api/directorysetting-update.md) | [<span data-ttu-id="9601f-132">directorySetting</span><span class="sxs-lookup"><span data-stu-id="9601f-132">directorySetting</span></span>](directorysetting.md)  |<span data-ttu-id="9601f-133">更新 setting 对象。</span><span class="sxs-lookup"><span data-stu-id="9601f-133">Update a setting object.</span></span> <span data-ttu-id="9601f-134">仅 settingValues 可以更新中更改。</span><span class="sxs-lookup"><span data-stu-id="9601f-134">Only settingValues can be changed in an update.</span></span>|
|[<span data-ttu-id="9601f-135">删除设置</span><span class="sxs-lookup"><span data-stu-id="9601f-135">Delete setting</span></span>](../api/directorysetting-delete.md) | <span data-ttu-id="9601f-136">无</span><span class="sxs-lookup"><span data-stu-id="9601f-136">None</span></span> |<span data-ttu-id="9601f-137">删除设置对象。</span><span class="sxs-lookup"><span data-stu-id="9601f-137">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9601f-138">属性</span><span class="sxs-lookup"><span data-stu-id="9601f-138">Properties</span></span>
| <span data-ttu-id="9601f-139">属性</span><span class="sxs-lookup"><span data-stu-id="9601f-139">Property</span></span>     | <span data-ttu-id="9601f-140">类型</span><span class="sxs-lookup"><span data-stu-id="9601f-140">Type</span></span>   |<span data-ttu-id="9601f-141">说明</span><span class="sxs-lookup"><span data-stu-id="9601f-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9601f-142">displayName</span><span class="sxs-lookup"><span data-stu-id="9601f-142">displayName</span></span>|<span data-ttu-id="9601f-143">string</span><span class="sxs-lookup"><span data-stu-id="9601f-143">string</span></span>|<span data-ttu-id="9601f-144">来自相关模板的此组设置的显示名称。</span><span class="sxs-lookup"><span data-stu-id="9601f-144">Display name of this group of settings, which comes from the associated template.</span></span> <span data-ttu-id="9601f-145">只读。</span><span class="sxs-lookup"><span data-stu-id="9601f-145">Read-only.</span></span>|
|<span data-ttu-id="9601f-146">id</span><span class="sxs-lookup"><span data-stu-id="9601f-146">id</span></span>|<span data-ttu-id="9601f-147">string</span><span class="sxs-lookup"><span data-stu-id="9601f-147">string</span></span>| <span data-ttu-id="9601f-p108">这些设置的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="9601f-p108">Unique identifier for these settings. Read-only.</span></span>|
|<span data-ttu-id="9601f-150">templateId</span><span class="sxs-lookup"><span data-stu-id="9601f-150">templateId</span></span>|<span data-ttu-id="9601f-151">string</span><span class="sxs-lookup"><span data-stu-id="9601f-151">string</span></span>| <span data-ttu-id="9601f-p109">用于创建此组设置的模板的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="9601f-p109">Unique identifier for the template used to create this group of settings. Read-only.</span></span>|
|<span data-ttu-id="9601f-154">values</span><span class="sxs-lookup"><span data-stu-id="9601f-154">values</span></span>|<span data-ttu-id="9601f-155">[settingValue](settingvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9601f-155">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="9601f-p110">名称值对的集合。必须包含并设置模板中定义的所有设置。</span><span class="sxs-lookup"><span data-stu-id="9601f-p110">Collection of name value pairs. Must contain and set all the settings defined in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9601f-158">关系</span><span class="sxs-lookup"><span data-stu-id="9601f-158">Relationships</span></span>
<span data-ttu-id="9601f-159">无</span><span class="sxs-lookup"><span data-stu-id="9601f-159">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9601f-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9601f-160">JSON representation</span></span>

<span data-ttu-id="9601f-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9601f-161">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "directorySetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
