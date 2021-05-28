---
title: groupSettingTemplate 资源类型
description: 组设置模板表示可供租户使用的系统定义的设置。
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: a7868538c13b1e386e7aa10dcdf3fed9c03b198f
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680869"
---
# <a name="groupsettingtemplate-resource-type"></a><span data-ttu-id="9d001-103">groupSettingTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d001-103">groupSettingTemplate resource type</span></span>

<span data-ttu-id="9d001-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d001-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9d001-105">组设置模板表示可供租户使用的系统定义的设置。</span><span class="sxs-lookup"><span data-stu-id="9d001-105">Group setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="9d001-106">[组设置](groupsetting.md) 可以基于可用的 **groupSettingTemplates** 创建，值会从预设默认值更改。</span><span class="sxs-lookup"><span data-stu-id="9d001-106">[Group settings](groupsetting.md) can be created based on the available **groupSettingTemplates**, and values changed from their preset defaults.</span></span> <span data-ttu-id="9d001-107">无法创建、更新或删除组设置模板。</span><span class="sxs-lookup"><span data-stu-id="9d001-107">Group setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="9d001-108">这些设置可以表示租户范围的设置，也可以表示特定的组设置。</span><span class="sxs-lookup"><span data-stu-id="9d001-108">These settings can represent tenant-wide settings, or can represent specific group settings.</span></span> <span data-ttu-id="9d001-109">目前，唯一可用的模板适用于Microsoft 365组，并包括诸如用户是否可以创建组或邀请组织外部的来宾成为组成员的设置。</span><span class="sxs-lookup"><span data-stu-id="9d001-109">Currently, the only templates available apply to Microsoft 365 groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

## <a name="methods"></a><span data-ttu-id="9d001-110">方法</span><span class="sxs-lookup"><span data-stu-id="9d001-110">Methods</span></span>

| <span data-ttu-id="9d001-111">方法</span><span class="sxs-lookup"><span data-stu-id="9d001-111">Method</span></span> | <span data-ttu-id="9d001-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="9d001-112">Return Type</span></span> | <span data-ttu-id="9d001-113">说明</span><span class="sxs-lookup"><span data-stu-id="9d001-113">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="9d001-114">获取 groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="9d001-114">Get groupSettingTemplate</span></span>](../api/groupsettingtemplate-get.md) | [<span data-ttu-id="9d001-115">groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="9d001-115">groupSettingTemplate</span></span>](groupsettingtemplate.md) | <span data-ttu-id="9d001-116">读取系统定义的 groupSettingTemplate 对象之一的特定属性。</span><span class="sxs-lookup"><span data-stu-id="9d001-116">Read the specific properties of one of the system defined groupSettingTemplate objects.</span></span> |
|[<span data-ttu-id="9d001-117">列出 groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="9d001-117">List groupSettingTemplate</span></span>](../api/groupsettingtemplate-list.md) | [<span data-ttu-id="9d001-118">groupSettingTemplate 的集合</span><span class="sxs-lookup"><span data-stu-id="9d001-118">Collection of groupSettingTemplate</span></span>](groupsettingtemplate.md) |<span data-ttu-id="9d001-119">列出所有系统定义的 groupSettingTemplate 对象。</span><span class="sxs-lookup"><span data-stu-id="9d001-119">List all of the system defined groupSettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="9d001-120">属性</span><span class="sxs-lookup"><span data-stu-id="9d001-120">Properties</span></span>

| <span data-ttu-id="9d001-121">属性</span><span class="sxs-lookup"><span data-stu-id="9d001-121">Property</span></span> | <span data-ttu-id="9d001-122">类型</span><span class="sxs-lookup"><span data-stu-id="9d001-122">Type</span></span> | <span data-ttu-id="9d001-123">说明</span><span class="sxs-lookup"><span data-stu-id="9d001-123">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9d001-124">说明</span><span class="sxs-lookup"><span data-stu-id="9d001-124">description</span></span>|<span data-ttu-id="9d001-125">String</span><span class="sxs-lookup"><span data-stu-id="9d001-125">String</span></span>| <span data-ttu-id="9d001-126">模板的说明。</span><span class="sxs-lookup"><span data-stu-id="9d001-126">Description of the template.</span></span> |
|<span data-ttu-id="9d001-127">displayName</span><span class="sxs-lookup"><span data-stu-id="9d001-127">displayName</span></span>|<span data-ttu-id="9d001-128">String</span><span class="sxs-lookup"><span data-stu-id="9d001-128">String</span></span>| <span data-ttu-id="9d001-129">模板的显示名称。</span><span class="sxs-lookup"><span data-stu-id="9d001-129">Display name of the template.</span></span> |
|<span data-ttu-id="9d001-130">id</span><span class="sxs-lookup"><span data-stu-id="9d001-130">id</span></span>|<span data-ttu-id="9d001-131">String</span><span class="sxs-lookup"><span data-stu-id="9d001-131">String</span></span>| <span data-ttu-id="9d001-132">模板的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9d001-132">Unique identifier for the template.</span></span> <span data-ttu-id="9d001-133">只读。</span><span class="sxs-lookup"><span data-stu-id="9d001-133">Read-only.</span></span>|
|<span data-ttu-id="9d001-134">values</span><span class="sxs-lookup"><span data-stu-id="9d001-134">values</span></span>|<span data-ttu-id="9d001-135">[settingTemplateValue](settingtemplatevalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9d001-135">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="9d001-136">settingTemplateValues 的集合，该集合列出了一组可用设置、默认值和类型，这些设置、默认值和类型是此模板的一部分。</span><span class="sxs-lookup"><span data-stu-id="9d001-136">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9d001-137">关系</span><span class="sxs-lookup"><span data-stu-id="9d001-137">Relationships</span></span>

<span data-ttu-id="9d001-138">无。</span><span class="sxs-lookup"><span data-stu-id="9d001-138">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="9d001-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d001-139">JSON representation</span></span>

<span data-ttu-id="9d001-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d001-140">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.groupSettingTemplate"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "values": [{"@odata.type": "microsoft.graph.settingTemplateValue"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupSettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

