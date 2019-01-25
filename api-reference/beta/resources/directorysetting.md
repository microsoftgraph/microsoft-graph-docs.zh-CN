---
title: directorySetting 资源类型
description: 可以创建基于可用 directorySettingTemplates，并从其预设的默认值更改目录设置。 这些设置可以控制实体或功能行为，同时在租户范围级别或特定实体级别。 在租户范围和特定实体级别定义相同的设置后，特定实体级别设置可能会选择退出从租户范围的设置。  例如，租户范围的设置可能允许来宾要邀请的现有组的成员，但的特定组设置可能会选择退出，并且不允许来宾要邀请的组的成员。 当前定义的系统设置是仅控制 Office 组行为。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b489bf1130bd91d28b3a2b41a78c38b881e90d27
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521367"
---
# <a name="directorysetting-resource-type"></a><span data-ttu-id="bdb3b-107">directorySetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="bdb3b-107">directorySetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdb3b-108">可以创建基于可用[directorySettingTemplates](directorysettingtemplate.md)，并从其预设的默认值更改目录设置。</span><span class="sxs-lookup"><span data-stu-id="bdb3b-108">Directory settings can be created based on the available [directorySettingTemplates](directorysettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="bdb3b-109">这些设置可以控制实体或功能行为，同时在租户范围级别或特定实体级别。</span><span class="sxs-lookup"><span data-stu-id="bdb3b-109">These settings can govern entity or feature behaviors, both at a tenant-wide level or at a specific entity level.</span></span> <span data-ttu-id="bdb3b-110">在租户范围和特定实体级别定义相同的设置后，特定实体级别设置可能会选择退出从租户范围的设置。</span><span class="sxs-lookup"><span data-stu-id="bdb3b-110">When the same setting is defined at both the tenant-wide and specific entity level, the specific entity level setting may opt-out from the tenant-wide setting.</span></span>  <span data-ttu-id="bdb3b-111">例如，租户范围的设置可能允许来宾要邀请的现有组的成员，但的特定组设置可能会选择退出，并且不允许来宾要邀请的组的成员。</span><span class="sxs-lookup"><span data-stu-id="bdb3b-111">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but a specific group setting may opt-out and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="bdb3b-112">当前定义的系统设置是仅控制 Office 组行为。</span><span class="sxs-lookup"><span data-stu-id="bdb3b-112">Currently system defined settings are only govern Office groups behavior.</span></span>

> <span data-ttu-id="bdb3b-113">**注意**： directorySetting 资源类型的 /beta 版本仅适用于组。</span><span class="sxs-lookup"><span data-stu-id="bdb3b-113">**Note**: The /beta version of the directorySetting resource type only applies to groups.</span></span> <span data-ttu-id="bdb3b-114">/V1.0 版本已被重命名为 groupSetting。</span><span class="sxs-lookup"><span data-stu-id="bdb3b-114">The /v1.0 version has been renamed to groupSetting.</span></span>

## <a name="methods"></a><span data-ttu-id="bdb3b-115">方法</span><span class="sxs-lookup"><span data-stu-id="bdb3b-115">Methods</span></span>

| <span data-ttu-id="bdb3b-116">方法</span><span class="sxs-lookup"><span data-stu-id="bdb3b-116">Method</span></span>           | <span data-ttu-id="bdb3b-117">返回类型</span><span class="sxs-lookup"><span data-stu-id="bdb3b-117">Return Type</span></span>    |<span data-ttu-id="bdb3b-118">说明</span><span class="sxs-lookup"><span data-stu-id="bdb3b-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bdb3b-119">Create setting</span><span class="sxs-lookup"><span data-stu-id="bdb3b-119">Create setting</span></span>](../api/directorysetting-post-settings.md) | [<span data-ttu-id="bdb3b-120">directorySetting</span><span class="sxs-lookup"><span data-stu-id="bdb3b-120">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="bdb3b-121">基于 directorySettingTemplate 创建设置对象。</span><span class="sxs-lookup"><span data-stu-id="bdb3b-121">Create a setting object based on a directorySettingTemplate.</span></span> <span data-ttu-id="bdb3b-122">POST 请求必须为模板中定义的所有设置提供 settingValues。</span><span class="sxs-lookup"><span data-stu-id="bdb3b-122">The POST request must provide settingValues for all the settings defined in the template.</span></span>|
|[<span data-ttu-id="bdb3b-123">Get setting</span><span class="sxs-lookup"><span data-stu-id="bdb3b-123">Get setting</span></span>](../api/directorysetting-get.md) | [<span data-ttu-id="bdb3b-124">directorySetting</span><span class="sxs-lookup"><span data-stu-id="bdb3b-124">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="bdb3b-125">读取特定设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bdb3b-125">Read properties of a specific setting object.</span></span>|
|[<span data-ttu-id="bdb3b-126">List settings</span><span class="sxs-lookup"><span data-stu-id="bdb3b-126">List settings</span></span>](../api/directorysetting-list.md) | <span data-ttu-id="bdb3b-127">[directorySetting](directorysetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bdb3b-127">[directorySetting](directorysetting.md) collection</span></span> |<span data-ttu-id="bdb3b-128">列出所有设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bdb3b-128">List properties of all setting objects.</span></span>|
|[<span data-ttu-id="bdb3b-129">Update setting</span><span class="sxs-lookup"><span data-stu-id="bdb3b-129">Update setting</span></span>](../api/directorysetting-update.md) | [<span data-ttu-id="bdb3b-130">directorySetting</span><span class="sxs-lookup"><span data-stu-id="bdb3b-130">directorySetting</span></span>](directorysetting.md)  |<span data-ttu-id="bdb3b-131">更新 setting 对象。</span><span class="sxs-lookup"><span data-stu-id="bdb3b-131">Update a setting object.</span></span> <span data-ttu-id="bdb3b-132">仅 settingValues 可以更新中更改。</span><span class="sxs-lookup"><span data-stu-id="bdb3b-132">Only settingValues can be changed in an update.</span></span>|
|[<span data-ttu-id="bdb3b-133">删除设置</span><span class="sxs-lookup"><span data-stu-id="bdb3b-133">Delete setting</span></span>](../api/directorysetting-delete.md) | <span data-ttu-id="bdb3b-134">无</span><span class="sxs-lookup"><span data-stu-id="bdb3b-134">None</span></span> |<span data-ttu-id="bdb3b-135">删除设置对象。</span><span class="sxs-lookup"><span data-stu-id="bdb3b-135">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="bdb3b-136">属性</span><span class="sxs-lookup"><span data-stu-id="bdb3b-136">Properties</span></span>
| <span data-ttu-id="bdb3b-137">属性</span><span class="sxs-lookup"><span data-stu-id="bdb3b-137">Property</span></span>     | <span data-ttu-id="bdb3b-138">类型</span><span class="sxs-lookup"><span data-stu-id="bdb3b-138">Type</span></span>   |<span data-ttu-id="bdb3b-139">说明</span><span class="sxs-lookup"><span data-stu-id="bdb3b-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bdb3b-140">displayName</span><span class="sxs-lookup"><span data-stu-id="bdb3b-140">displayName</span></span>|<span data-ttu-id="bdb3b-141">string</span><span class="sxs-lookup"><span data-stu-id="bdb3b-141">string</span></span>|<span data-ttu-id="bdb3b-142">来自相关模板的此组设置的显示名称。</span><span class="sxs-lookup"><span data-stu-id="bdb3b-142">Display name of this group of settings, which comes from the associated template.</span></span> <span data-ttu-id="bdb3b-143">只读。</span><span class="sxs-lookup"><span data-stu-id="bdb3b-143">Read-only.</span></span>|
|<span data-ttu-id="bdb3b-144">id</span><span class="sxs-lookup"><span data-stu-id="bdb3b-144">id</span></span>|<span data-ttu-id="bdb3b-145">string</span><span class="sxs-lookup"><span data-stu-id="bdb3b-145">string</span></span>| <span data-ttu-id="bdb3b-p107">这些设置的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="bdb3b-p107">Unique identifier for these settings. Read-only.</span></span>|
|<span data-ttu-id="bdb3b-148">templateId</span><span class="sxs-lookup"><span data-stu-id="bdb3b-148">templateId</span></span>|<span data-ttu-id="bdb3b-149">string</span><span class="sxs-lookup"><span data-stu-id="bdb3b-149">string</span></span>| <span data-ttu-id="bdb3b-p108">用于创建此组设置的模板的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="bdb3b-p108">Unique identifier for the template used to create this group of settings. Read-only.</span></span>|
|<span data-ttu-id="bdb3b-152">values</span><span class="sxs-lookup"><span data-stu-id="bdb3b-152">values</span></span>|<span data-ttu-id="bdb3b-153">[settingValue](settingvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bdb3b-153">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="bdb3b-p109">名称值对的集合。必须包含并设置模板中定义的所有设置。</span><span class="sxs-lookup"><span data-stu-id="bdb3b-p109">Collection of name value pairs. Must contain and set all the settings defined in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bdb3b-156">关系</span><span class="sxs-lookup"><span data-stu-id="bdb3b-156">Relationships</span></span>
<span data-ttu-id="bdb3b-157">无</span><span class="sxs-lookup"><span data-stu-id="bdb3b-157">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="bdb3b-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bdb3b-158">JSON representation</span></span>

<span data-ttu-id="bdb3b-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bdb3b-159">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/directorysetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
