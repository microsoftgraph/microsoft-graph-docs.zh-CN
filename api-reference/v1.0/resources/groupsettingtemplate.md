---
title: groupSettingTemplate 资源类型
description: 组设置模板表示对租户可用的系统定义设置。 可以基于可用的**groupSettingTemplates**创建组设置，并将值更改为其预设默认值。 无法创建、更新或删除组设置模板。 这些设置可以表示租户范围的设置，也可以表示特定的组设置。 目前，仅有的可用模板适用于 Office 365 组，并包括一些设置，例如，用户是否可以创建组或邀请来自组织外部的来宾成为组的成员。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fa392d6bf6dcd8ceaf15d97dfe695fbaaeabed4b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531359"
---
# <a name="groupsettingtemplate-resource-type"></a><span data-ttu-id="af2c5-107">groupSettingTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="af2c5-107">groupSettingTemplate resource type</span></span>

<span data-ttu-id="af2c5-108">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af2c5-108">Namespace: microsoft.graph</span></span>

<span data-ttu-id="af2c5-109">组设置模板表示对租户可用的系统定义设置。</span><span class="sxs-lookup"><span data-stu-id="af2c5-109">Group setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="af2c5-110">可以基于可用的**groupSettingTemplates**创建[组设置](groupsetting.md)，并将值更改为其预设默认值。</span><span class="sxs-lookup"><span data-stu-id="af2c5-110">[Group settings](groupsetting.md) can be created based on the available **groupSettingTemplates**, and values changed from their preset defaults.</span></span> <span data-ttu-id="af2c5-111">无法创建、更新或删除组设置模板。</span><span class="sxs-lookup"><span data-stu-id="af2c5-111">Group setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="af2c5-112">这些设置可以表示租户范围的设置，也可以表示特定的组设置。</span><span class="sxs-lookup"><span data-stu-id="af2c5-112">These settings can represent tenant-wide settings, or can represent specific group settings.</span></span> <span data-ttu-id="af2c5-113">目前，仅有的可用模板适用于 Office 365 组，并包括一些设置，例如，用户是否可以创建组或邀请来自组织外部的来宾成为组的成员。</span><span class="sxs-lookup"><span data-stu-id="af2c5-113">Currently, the only templates available apply to Office 365 groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

## <a name="methods"></a><span data-ttu-id="af2c5-114">Methods</span><span class="sxs-lookup"><span data-stu-id="af2c5-114">Methods</span></span>

| <span data-ttu-id="af2c5-115">方法</span><span class="sxs-lookup"><span data-stu-id="af2c5-115">Method</span></span> | <span data-ttu-id="af2c5-116">返回类型</span><span class="sxs-lookup"><span data-stu-id="af2c5-116">Return Type</span></span> | <span data-ttu-id="af2c5-117">说明</span><span class="sxs-lookup"><span data-stu-id="af2c5-117">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="af2c5-118">获取 groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="af2c5-118">Get groupSettingTemplate</span></span>](../api/groupsettingtemplate-get.md) | [<span data-ttu-id="af2c5-119">groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="af2c5-119">groupSettingTemplate</span></span>](groupsettingtemplate.md) | <span data-ttu-id="af2c5-120">读取某个系统定义的 groupSettingTemplate 对象的特定属性。</span><span class="sxs-lookup"><span data-stu-id="af2c5-120">Read the specific properties of one of the system defined groupSettingTemplate objects.</span></span> |
|[<span data-ttu-id="af2c5-121">列出 groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="af2c5-121">List groupSettingTemplate</span></span>](../api/groupsettingtemplate-list.md) | [<span data-ttu-id="af2c5-122">GroupSettingTemplate 的集合</span><span class="sxs-lookup"><span data-stu-id="af2c5-122">Collection of groupSettingTemplate</span></span>](groupsettingtemplate.md) |<span data-ttu-id="af2c5-123">列出所有系统定义的 groupSettingTemplate 对象。</span><span class="sxs-lookup"><span data-stu-id="af2c5-123">List all of the system defined groupSettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="af2c5-124">属性</span><span class="sxs-lookup"><span data-stu-id="af2c5-124">Properties</span></span>

| <span data-ttu-id="af2c5-125">属性</span><span class="sxs-lookup"><span data-stu-id="af2c5-125">Property</span></span> | <span data-ttu-id="af2c5-126">类型</span><span class="sxs-lookup"><span data-stu-id="af2c5-126">Type</span></span> | <span data-ttu-id="af2c5-127">说明</span><span class="sxs-lookup"><span data-stu-id="af2c5-127">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="af2c5-128">说明</span><span class="sxs-lookup"><span data-stu-id="af2c5-128">description</span></span>|<span data-ttu-id="af2c5-129">String</span><span class="sxs-lookup"><span data-stu-id="af2c5-129">String</span></span>| <span data-ttu-id="af2c5-130">模板的说明。</span><span class="sxs-lookup"><span data-stu-id="af2c5-130">Description of the template.</span></span> |
|<span data-ttu-id="af2c5-131">displayName</span><span class="sxs-lookup"><span data-stu-id="af2c5-131">displayName</span></span>|<span data-ttu-id="af2c5-132">String</span><span class="sxs-lookup"><span data-stu-id="af2c5-132">String</span></span>| <span data-ttu-id="af2c5-133">模板的显示名称。</span><span class="sxs-lookup"><span data-stu-id="af2c5-133">Display name of the template.</span></span> |
|<span data-ttu-id="af2c5-134">id</span><span class="sxs-lookup"><span data-stu-id="af2c5-134">id</span></span>|<span data-ttu-id="af2c5-135">字符串</span><span class="sxs-lookup"><span data-stu-id="af2c5-135">String</span></span>| <span data-ttu-id="af2c5-136">模板的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="af2c5-136">Unique identifier for the template.</span></span> <span data-ttu-id="af2c5-137">只读。</span><span class="sxs-lookup"><span data-stu-id="af2c5-137">Read-only.</span></span>|
|<span data-ttu-id="af2c5-138">values</span><span class="sxs-lookup"><span data-stu-id="af2c5-138">values</span></span>|<span data-ttu-id="af2c5-139">[settingTemplateValue](settingtemplatevalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="af2c5-139">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="af2c5-140">Settemplatevalues 的集合，该集合列出了组成此模板的可用设置、默认值和类型的集合。</span><span class="sxs-lookup"><span data-stu-id="af2c5-140">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="af2c5-141">关系</span><span class="sxs-lookup"><span data-stu-id="af2c5-141">Relationships</span></span>

<span data-ttu-id="af2c5-142">无。</span><span class="sxs-lookup"><span data-stu-id="af2c5-142">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="af2c5-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="af2c5-143">JSON representation</span></span>

<span data-ttu-id="af2c5-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af2c5-144">Here is a JSON representation of the resource.</span></span>

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
