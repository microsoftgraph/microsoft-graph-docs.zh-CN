---
title: groupSettingTemplate 资源类型
description: 组设置模板表示对租户可用的系统定义设置。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: f103ae27065701951cb7a7881ebaa898d455243c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48062930"
---
# <a name="groupsettingtemplate-resource-type"></a><span data-ttu-id="8b8e6-103">groupSettingTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="8b8e6-103">groupSettingTemplate resource type</span></span>

<span data-ttu-id="8b8e6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b8e6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8b8e6-105">组设置模板表示对租户可用的系统定义设置。</span><span class="sxs-lookup"><span data-stu-id="8b8e6-105">Group setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="8b8e6-106">可以基于可用的**groupSettingTemplates**创建[组设置](groupsetting.md)，并将值更改为其预设默认值。</span><span class="sxs-lookup"><span data-stu-id="8b8e6-106">[Group settings](groupsetting.md) can be created based on the available **groupSettingTemplates**, and values changed from their preset defaults.</span></span> <span data-ttu-id="8b8e6-107">无法创建、更新或删除组设置模板。</span><span class="sxs-lookup"><span data-stu-id="8b8e6-107">Group setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="8b8e6-108">这些设置可以表示租户范围的设置，也可以表示特定的组设置。</span><span class="sxs-lookup"><span data-stu-id="8b8e6-108">These settings can represent tenant-wide settings, or can represent specific group settings.</span></span> <span data-ttu-id="8b8e6-109">目前，仅有的可用模板适用于 Microsoft 365 组，并包括一些设置，例如，用户是否可以创建组或邀请来自组织外部的来宾成为组的成员。</span><span class="sxs-lookup"><span data-stu-id="8b8e6-109">Currently, the only templates available apply to Microsoft 365 groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

## <a name="methods"></a><span data-ttu-id="8b8e6-110">方法</span><span class="sxs-lookup"><span data-stu-id="8b8e6-110">Methods</span></span>

| <span data-ttu-id="8b8e6-111">方法</span><span class="sxs-lookup"><span data-stu-id="8b8e6-111">Method</span></span> | <span data-ttu-id="8b8e6-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="8b8e6-112">Return Type</span></span> | <span data-ttu-id="8b8e6-113">说明</span><span class="sxs-lookup"><span data-stu-id="8b8e6-113">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="8b8e6-114">获取 groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="8b8e6-114">Get groupSettingTemplate</span></span>](../api/groupsettingtemplate-get.md) | [<span data-ttu-id="8b8e6-115">groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="8b8e6-115">groupSettingTemplate</span></span>](groupsettingtemplate.md) | <span data-ttu-id="8b8e6-116">读取某个系统定义的 groupSettingTemplate 对象的特定属性。</span><span class="sxs-lookup"><span data-stu-id="8b8e6-116">Read the specific properties of one of the system defined groupSettingTemplate objects.</span></span> |
|[<span data-ttu-id="8b8e6-117">列出 groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="8b8e6-117">List groupSettingTemplate</span></span>](../api/groupsettingtemplate-list.md) | [<span data-ttu-id="8b8e6-118">GroupSettingTemplate 的集合</span><span class="sxs-lookup"><span data-stu-id="8b8e6-118">Collection of groupSettingTemplate</span></span>](groupsettingtemplate.md) |<span data-ttu-id="8b8e6-119">列出所有系统定义的 groupSettingTemplate 对象。</span><span class="sxs-lookup"><span data-stu-id="8b8e6-119">List all of the system defined groupSettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="8b8e6-120">属性</span><span class="sxs-lookup"><span data-stu-id="8b8e6-120">Properties</span></span>

| <span data-ttu-id="8b8e6-121">属性</span><span class="sxs-lookup"><span data-stu-id="8b8e6-121">Property</span></span> | <span data-ttu-id="8b8e6-122">类型</span><span class="sxs-lookup"><span data-stu-id="8b8e6-122">Type</span></span> | <span data-ttu-id="8b8e6-123">说明</span><span class="sxs-lookup"><span data-stu-id="8b8e6-123">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8b8e6-124">说明</span><span class="sxs-lookup"><span data-stu-id="8b8e6-124">description</span></span>|<span data-ttu-id="8b8e6-125">String</span><span class="sxs-lookup"><span data-stu-id="8b8e6-125">String</span></span>| <span data-ttu-id="8b8e6-126">模板的说明。</span><span class="sxs-lookup"><span data-stu-id="8b8e6-126">Description of the template.</span></span> |
|<span data-ttu-id="8b8e6-127">displayName</span><span class="sxs-lookup"><span data-stu-id="8b8e6-127">displayName</span></span>|<span data-ttu-id="8b8e6-128">String</span><span class="sxs-lookup"><span data-stu-id="8b8e6-128">String</span></span>| <span data-ttu-id="8b8e6-129">模板的显示名称。</span><span class="sxs-lookup"><span data-stu-id="8b8e6-129">Display name of the template.</span></span> |
|<span data-ttu-id="8b8e6-130">id</span><span class="sxs-lookup"><span data-stu-id="8b8e6-130">id</span></span>|<span data-ttu-id="8b8e6-131">String</span><span class="sxs-lookup"><span data-stu-id="8b8e6-131">String</span></span>| <span data-ttu-id="8b8e6-132">模板的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8b8e6-132">Unique identifier for the template.</span></span> <span data-ttu-id="8b8e6-133">只读。</span><span class="sxs-lookup"><span data-stu-id="8b8e6-133">Read-only.</span></span>|
|<span data-ttu-id="8b8e6-134">values</span><span class="sxs-lookup"><span data-stu-id="8b8e6-134">values</span></span>|<span data-ttu-id="8b8e6-135">[settingTemplateValue](settingtemplatevalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8b8e6-135">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="8b8e6-136">Settemplatevalues 的集合，该集合列出了组成此模板的可用设置、默认值和类型的集合。</span><span class="sxs-lookup"><span data-stu-id="8b8e6-136">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8b8e6-137">关系</span><span class="sxs-lookup"><span data-stu-id="8b8e6-137">Relationships</span></span>

<span data-ttu-id="8b8e6-138">无。</span><span class="sxs-lookup"><span data-stu-id="8b8e6-138">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="8b8e6-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8b8e6-139">JSON representation</span></span>

<span data-ttu-id="8b8e6-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8b8e6-140">Here is a JSON representation of the resource.</span></span>

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

