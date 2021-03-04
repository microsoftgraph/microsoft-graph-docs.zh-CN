---
title: directorySetting 资源类型
description: 目录设置可基于可用的 directorySettingTemplates 创建，并更改其预设默认值。
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 50c73e9c68cd3d2fa3f4aed6c7eba84141443d1a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440449"
---
# <a name="directorysetting-resource-type"></a><span data-ttu-id="009d1-103">directorySetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="009d1-103">directorySetting resource type</span></span>

<span data-ttu-id="009d1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="009d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="009d1-105">目录设置可以基于可用的 [directorySettingTemplates](directorysettingtemplate.md)创建，并更改其预设默认值。</span><span class="sxs-lookup"><span data-stu-id="009d1-105">Directory settings can be created based on the available [directorySettingTemplates](directorysettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="009d1-106">这些设置可以在租户范围内或特定实体级别管理实体或功能行为。</span><span class="sxs-lookup"><span data-stu-id="009d1-106">These settings can govern entity or feature behaviors, both at a tenant-wide level or at a specific entity level.</span></span> <span data-ttu-id="009d1-107">当在租户范围和特定实体级别定义相同设置时，特定实体级别设置可能会选择从租户范围的设置中退出。</span><span class="sxs-lookup"><span data-stu-id="009d1-107">When the same setting is defined at both the tenant-wide and specific entity level, the specific entity level setting may opt-out from the tenant-wide setting.</span></span>  <span data-ttu-id="009d1-108">例如，租户范围的设置可能允许现有组成员邀请来宾，但特定组设置可能会选择退出，并且不允许组的成员邀请来宾。</span><span class="sxs-lookup"><span data-stu-id="009d1-108">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but a specific group setting may opt-out and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="009d1-109">目前，系统定义的设置仅控制 Office 组行为。</span><span class="sxs-lookup"><span data-stu-id="009d1-109">Currently system defined settings are only govern Office groups behavior.</span></span>

> <span data-ttu-id="009d1-110">**注意**：directorySetting 资源类型的 /beta 版本仅适用于组。</span><span class="sxs-lookup"><span data-stu-id="009d1-110">**Note**: The /beta version of the directorySetting resource type only applies to groups.</span></span> <span data-ttu-id="009d1-111">/v1.0 版本已重命名为 groupSetting。</span><span class="sxs-lookup"><span data-stu-id="009d1-111">The /v1.0 version has been renamed to groupSetting.</span></span>

## <a name="methods"></a><span data-ttu-id="009d1-112">Methods</span><span class="sxs-lookup"><span data-stu-id="009d1-112">Methods</span></span>

| <span data-ttu-id="009d1-113">方法</span><span class="sxs-lookup"><span data-stu-id="009d1-113">Method</span></span>           | <span data-ttu-id="009d1-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="009d1-114">Return Type</span></span>    |<span data-ttu-id="009d1-115">说明</span><span class="sxs-lookup"><span data-stu-id="009d1-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="009d1-116">Create setting</span><span class="sxs-lookup"><span data-stu-id="009d1-116">Create setting</span></span>](../api/directorysetting-post-settings.md) | [<span data-ttu-id="009d1-117">directorySetting</span><span class="sxs-lookup"><span data-stu-id="009d1-117">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="009d1-118">创建基于 directorySettingTemplate 的设置对象。</span><span class="sxs-lookup"><span data-stu-id="009d1-118">Create a setting object based on a directorySettingTemplate.</span></span> <span data-ttu-id="009d1-119">POST 请求必须提供模板中定义的所有设置的 settingValues。</span><span class="sxs-lookup"><span data-stu-id="009d1-119">The POST request must provide settingValues for all the settings defined in the template.</span></span>|
|[<span data-ttu-id="009d1-120">Get setting</span><span class="sxs-lookup"><span data-stu-id="009d1-120">Get setting</span></span>](../api/directorysetting-get.md) | [<span data-ttu-id="009d1-121">directorySetting</span><span class="sxs-lookup"><span data-stu-id="009d1-121">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="009d1-122">读取特定设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="009d1-122">Read properties of a specific setting object.</span></span>|
|[<span data-ttu-id="009d1-123">List settings</span><span class="sxs-lookup"><span data-stu-id="009d1-123">List settings</span></span>](../api/directorysetting-list.md) | <span data-ttu-id="009d1-124">[directorySetting](directorysetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="009d1-124">[directorySetting](directorysetting.md) collection</span></span> |<span data-ttu-id="009d1-125">列出所有设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="009d1-125">List properties of all setting objects.</span></span>|
|[<span data-ttu-id="009d1-126">Update setting</span><span class="sxs-lookup"><span data-stu-id="009d1-126">Update setting</span></span>](../api/directorysetting-update.md) | [<span data-ttu-id="009d1-127">directorySetting</span><span class="sxs-lookup"><span data-stu-id="009d1-127">directorySetting</span></span>](directorysetting.md)  |<span data-ttu-id="009d1-128">更新 setting 对象。</span><span class="sxs-lookup"><span data-stu-id="009d1-128">Update a setting object.</span></span> <span data-ttu-id="009d1-129">更新中只能更改 settingValues。</span><span class="sxs-lookup"><span data-stu-id="009d1-129">Only settingValues can be changed in an update.</span></span>|
|[<span data-ttu-id="009d1-130">删除设置</span><span class="sxs-lookup"><span data-stu-id="009d1-130">Delete setting</span></span>](../api/directorysetting-delete.md) | <span data-ttu-id="009d1-131">无</span><span class="sxs-lookup"><span data-stu-id="009d1-131">None</span></span> |<span data-ttu-id="009d1-132">删除 setting 对象。</span><span class="sxs-lookup"><span data-stu-id="009d1-132">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="009d1-133">属性</span><span class="sxs-lookup"><span data-stu-id="009d1-133">Properties</span></span>
| <span data-ttu-id="009d1-134">属性</span><span class="sxs-lookup"><span data-stu-id="009d1-134">Property</span></span>     | <span data-ttu-id="009d1-135">类型</span><span class="sxs-lookup"><span data-stu-id="009d1-135">Type</span></span>   |<span data-ttu-id="009d1-136">说明</span><span class="sxs-lookup"><span data-stu-id="009d1-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="009d1-137">displayName</span><span class="sxs-lookup"><span data-stu-id="009d1-137">displayName</span></span>|<span data-ttu-id="009d1-138">string</span><span class="sxs-lookup"><span data-stu-id="009d1-138">string</span></span>|<span data-ttu-id="009d1-139">来自关联模板的这组设置的显示名称。</span><span class="sxs-lookup"><span data-stu-id="009d1-139">Display name of this group of settings, which comes from the associated template.</span></span> <span data-ttu-id="009d1-140">只读。</span><span class="sxs-lookup"><span data-stu-id="009d1-140">Read-only.</span></span>|
|<span data-ttu-id="009d1-141">id</span><span class="sxs-lookup"><span data-stu-id="009d1-141">id</span></span>|<span data-ttu-id="009d1-142">string</span><span class="sxs-lookup"><span data-stu-id="009d1-142">string</span></span>| <span data-ttu-id="009d1-143">这些设置的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="009d1-143">Unique identifier for these settings.</span></span> <span data-ttu-id="009d1-144">只读。</span><span class="sxs-lookup"><span data-stu-id="009d1-144">Read-only.</span></span>|
|<span data-ttu-id="009d1-145">templateId</span><span class="sxs-lookup"><span data-stu-id="009d1-145">templateId</span></span>|<span data-ttu-id="009d1-146">string</span><span class="sxs-lookup"><span data-stu-id="009d1-146">string</span></span>| <span data-ttu-id="009d1-147">用于创建此组设置的模板的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="009d1-147">Unique identifier for the template used to create this group of settings.</span></span> <span data-ttu-id="009d1-148">只读。</span><span class="sxs-lookup"><span data-stu-id="009d1-148">Read-only.</span></span>|
|<span data-ttu-id="009d1-149">values</span><span class="sxs-lookup"><span data-stu-id="009d1-149">values</span></span>|<span data-ttu-id="009d1-150">[settingValue](settingvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="009d1-150">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="009d1-151">名称值对的集合。</span><span class="sxs-lookup"><span data-stu-id="009d1-151">Collection of name value pairs.</span></span> <span data-ttu-id="009d1-152">必须包含和设置模板中定义的所有设置。</span><span class="sxs-lookup"><span data-stu-id="009d1-152">Must contain and set all the settings defined in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="009d1-153">关系</span><span class="sxs-lookup"><span data-stu-id="009d1-153">Relationships</span></span>
<span data-ttu-id="009d1-154">无</span><span class="sxs-lookup"><span data-stu-id="009d1-154">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="009d1-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="009d1-155">JSON representation</span></span>

<span data-ttu-id="009d1-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="009d1-156">Here is a JSON representation of the resource.</span></span>

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


