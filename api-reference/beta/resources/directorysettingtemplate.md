---
title: directorySettingTemplate 资源类型
description: 目录设置模板表示可供租户使用的系统定义的设置。
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 71984d472aab9f78197134fae0668fd0a90d7716
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440407"
---
# <a name="directorysettingtemplate-resource-type"></a><span data-ttu-id="deda5-103">directorySettingTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="deda5-103">directorySettingTemplate resource type</span></span>

<span data-ttu-id="deda5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="deda5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="deda5-105">目录设置模板表示可供租户使用的系统定义的设置。</span><span class="sxs-lookup"><span data-stu-id="deda5-105">Directory setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="deda5-106">[目录设置](directorysetting.md) 可以基于可用的 directorySettingTemplates 创建，并且值会从预设默认值更改。</span><span class="sxs-lookup"><span data-stu-id="deda5-106">[Directory settings](directorysetting.md) can be created based on the available directorySettingTemplates, and values changed from their preset defaults.</span></span> <span data-ttu-id="deda5-107">无法创建、更新或删除目录设置模板。</span><span class="sxs-lookup"><span data-stu-id="deda5-107">Directory setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="deda5-108">这些设置可以表示租户范围的设置，也可以表示特定的实体设置。</span><span class="sxs-lookup"><span data-stu-id="deda5-108">These settings can represent tenant-wide settings, or can represent specific entity settings.</span></span>  <span data-ttu-id="deda5-109">目前，唯一可用的模板适用于 Office 组，并包括设置，例如用户是否可以创建组或邀请组织外部的来宾成为组的成员。</span><span class="sxs-lookup"><span data-stu-id="deda5-109">Currently, the only templates available apply to Office groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

> <span data-ttu-id="deda5-110">**注意**：directorySettingTemplate 资源类型的 /beta 版本仅适用于组。</span><span class="sxs-lookup"><span data-stu-id="deda5-110">**Note**: The /beta version of the directorySettingTemplate resource type only applies to groups.</span></span> <span data-ttu-id="deda5-111">/v1.0 版本已重命名为 groupSettingTemplate。</span><span class="sxs-lookup"><span data-stu-id="deda5-111">The /v1.0 version has been renamed to groupSettingTemplate.</span></span>

## <a name="methods"></a><span data-ttu-id="deda5-112">Methods</span><span class="sxs-lookup"><span data-stu-id="deda5-112">Methods</span></span>

| <span data-ttu-id="deda5-113">方法</span><span class="sxs-lookup"><span data-stu-id="deda5-113">Method</span></span>           | <span data-ttu-id="deda5-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="deda5-114">Return Type</span></span>    |<span data-ttu-id="deda5-115">说明</span><span class="sxs-lookup"><span data-stu-id="deda5-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="deda5-116">获取 directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="deda5-116">Get directorySettingTemplate</span></span>](../api/directorysettingtemplate-get.md) | [<span data-ttu-id="deda5-117">directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="deda5-117">directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="deda5-118">读取系统定义的 directorySettingTemplate 对象之一的特定属性。</span><span class="sxs-lookup"><span data-stu-id="deda5-118">Read the specific properties of one of the system defined directorySettingTemplate objects.</span></span>|
|[<span data-ttu-id="deda5-119">列出 directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="deda5-119">List directorySettingTemplate</span></span>](../api/directorysettingtemplate-list.md) | [<span data-ttu-id="deda5-120">directorySettingTemplate 的集合</span><span class="sxs-lookup"><span data-stu-id="deda5-120">Collection of directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="deda5-121">列出所有系统定义的 directorySettingTemplate 对象。</span><span class="sxs-lookup"><span data-stu-id="deda5-121">List all of the system defined directorySettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="deda5-122">属性</span><span class="sxs-lookup"><span data-stu-id="deda5-122">Properties</span></span>
| <span data-ttu-id="deda5-123">属性</span><span class="sxs-lookup"><span data-stu-id="deda5-123">Property</span></span>     | <span data-ttu-id="deda5-124">类型</span><span class="sxs-lookup"><span data-stu-id="deda5-124">Type</span></span>   |<span data-ttu-id="deda5-125">说明</span><span class="sxs-lookup"><span data-stu-id="deda5-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="deda5-126">说明</span><span class="sxs-lookup"><span data-stu-id="deda5-126">description</span></span>|<span data-ttu-id="deda5-127">string</span><span class="sxs-lookup"><span data-stu-id="deda5-127">string</span></span>|<span data-ttu-id="deda5-128">模板的说明。</span><span class="sxs-lookup"><span data-stu-id="deda5-128">Description of the template.</span></span> <span data-ttu-id="deda5-129">只读。</span><span class="sxs-lookup"><span data-stu-id="deda5-129">Read-only.</span></span>|
|<span data-ttu-id="deda5-130">displayName</span><span class="sxs-lookup"><span data-stu-id="deda5-130">displayName</span></span>|<span data-ttu-id="deda5-131">string</span><span class="sxs-lookup"><span data-stu-id="deda5-131">string</span></span>|<span data-ttu-id="deda5-132">模板的显示名称。</span><span class="sxs-lookup"><span data-stu-id="deda5-132">Display name of the template.</span></span> <span data-ttu-id="deda5-133">只读。</span><span class="sxs-lookup"><span data-stu-id="deda5-133">Read-only.</span></span> |
|<span data-ttu-id="deda5-134">id</span><span class="sxs-lookup"><span data-stu-id="deda5-134">id</span></span>|<span data-ttu-id="deda5-135">string</span><span class="sxs-lookup"><span data-stu-id="deda5-135">string</span></span>| <span data-ttu-id="deda5-136">模板的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="deda5-136">Unique identifier for the template.</span></span> <span data-ttu-id="deda5-137">只读。</span><span class="sxs-lookup"><span data-stu-id="deda5-137">Read-only.</span></span>|
|<span data-ttu-id="deda5-138">values</span><span class="sxs-lookup"><span data-stu-id="deda5-138">values</span></span>|<span data-ttu-id="deda5-139">[settingTemplateValue](settingtemplatevalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="deda5-139">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="deda5-140">settingTemplateValues 的集合，列出一组可用设置、默认值和类型，这些设置、默认值和类型是此模板的一部分。</span><span class="sxs-lookup"><span data-stu-id="deda5-140">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span>  <span data-ttu-id="deda5-141">只读。</span><span class="sxs-lookup"><span data-stu-id="deda5-141">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="deda5-142">关系</span><span class="sxs-lookup"><span data-stu-id="deda5-142">Relationships</span></span>
<span data-ttu-id="deda5-143">无</span><span class="sxs-lookup"><span data-stu-id="deda5-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="deda5-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="deda5-144">JSON representation</span></span>

<span data-ttu-id="deda5-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="deda5-145">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySettingTemplate"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "values": [{"@odata.type": "microsoft.graph.settingTemplateValue"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directorySettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


