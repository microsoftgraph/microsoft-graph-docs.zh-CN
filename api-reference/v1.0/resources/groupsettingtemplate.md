---
title: groupSettingTemplate 资源类型
description: 组设置模板表示对租户可用的系统定义设置。 可以基于可用的**groupSettingTemplates**创建组设置, 并将值更改为其预设默认值。 无法创建、更新或删除组设置模板。 这些设置可以表示租户范围的设置, 也可以表示特定的组设置。 目前, 仅有的可用模板适用于 Office 365 组, 并包括一些设置, 例如, 用户是否可以创建组或邀请来自组织外部的来宾成为组的成员。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2b9b95303b72bc111f045010e71459f541e9a9b8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570790"
---
# <a name="groupsettingtemplate-resource-type"></a><span data-ttu-id="22aec-107">groupSettingTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="22aec-107">groupSettingTemplate resource type</span></span>

<span data-ttu-id="22aec-108">组设置模板表示对租户可用的系统定义设置。</span><span class="sxs-lookup"><span data-stu-id="22aec-108">Group setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="22aec-109">可以基于可用的**groupSettingTemplates**创建[组设置](groupsetting.md), 并将值更改为其预设默认值。</span><span class="sxs-lookup"><span data-stu-id="22aec-109">[Group settings](groupsetting.md) can be created based on the available **groupSettingTemplates**, and values changed from their preset defaults.</span></span> <span data-ttu-id="22aec-110">无法创建、更新或删除组设置模板。</span><span class="sxs-lookup"><span data-stu-id="22aec-110">Group setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="22aec-111">这些设置可以表示租户范围的设置, 也可以表示特定的组设置。</span><span class="sxs-lookup"><span data-stu-id="22aec-111">These settings can represent tenant-wide settings, or can represent specific group settings.</span></span> <span data-ttu-id="22aec-112">目前, 仅有的可用模板适用于 Office 365 组, 并包括一些设置, 例如, 用户是否可以创建组或邀请来自组织外部的来宾成为组的成员。</span><span class="sxs-lookup"><span data-stu-id="22aec-112">Currently, the only templates available apply to Office 365 groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

## <a name="methods"></a><span data-ttu-id="22aec-113">方法</span><span class="sxs-lookup"><span data-stu-id="22aec-113">Methods</span></span>

| <span data-ttu-id="22aec-114">方法</span><span class="sxs-lookup"><span data-stu-id="22aec-114">Method</span></span> | <span data-ttu-id="22aec-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="22aec-115">Return Type</span></span> | <span data-ttu-id="22aec-116">说明</span><span class="sxs-lookup"><span data-stu-id="22aec-116">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="22aec-117">获取 groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="22aec-117">Get groupSettingTemplate</span></span>](../api/groupsettingtemplate-get.md) | [<span data-ttu-id="22aec-118">groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="22aec-118">groupSettingTemplate</span></span>](groupsettingtemplate.md) | <span data-ttu-id="22aec-119">读取某个系统定义的 groupSettingTemplate 对象的特定属性。</span><span class="sxs-lookup"><span data-stu-id="22aec-119">Read the specific properties of one of the system defined groupSettingTemplate objects.</span></span> |
|[<span data-ttu-id="22aec-120">列出 groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="22aec-120">List groupSettingTemplate</span></span>](../api/groupsettingtemplate-list.md) | [<span data-ttu-id="22aec-121">groupSettingTemplate 的集合</span><span class="sxs-lookup"><span data-stu-id="22aec-121">Collection of groupSettingTemplate</span></span>](groupsettingtemplate.md) |<span data-ttu-id="22aec-122">列出所有系统定义的 groupSettingTemplate 对象。</span><span class="sxs-lookup"><span data-stu-id="22aec-122">List all of the system defined groupSettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="22aec-123">属性</span><span class="sxs-lookup"><span data-stu-id="22aec-123">Properties</span></span>

| <span data-ttu-id="22aec-124">属性</span><span class="sxs-lookup"><span data-stu-id="22aec-124">Property</span></span> | <span data-ttu-id="22aec-125">类型</span><span class="sxs-lookup"><span data-stu-id="22aec-125">Type</span></span> | <span data-ttu-id="22aec-126">说明</span><span class="sxs-lookup"><span data-stu-id="22aec-126">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="22aec-127">说明</span><span class="sxs-lookup"><span data-stu-id="22aec-127">description</span></span>|<span data-ttu-id="22aec-128">String</span><span class="sxs-lookup"><span data-stu-id="22aec-128">String</span></span>| <span data-ttu-id="22aec-129">模板的说明。</span><span class="sxs-lookup"><span data-stu-id="22aec-129">Description of the template.</span></span> |
|<span data-ttu-id="22aec-130">displayName</span><span class="sxs-lookup"><span data-stu-id="22aec-130">displayName</span></span>|<span data-ttu-id="22aec-131">String</span><span class="sxs-lookup"><span data-stu-id="22aec-131">String</span></span>| <span data-ttu-id="22aec-132">模板的显示名称。</span><span class="sxs-lookup"><span data-stu-id="22aec-132">Display name of the template.</span></span> |
|<span data-ttu-id="22aec-133">id</span><span class="sxs-lookup"><span data-stu-id="22aec-133">id</span></span>|<span data-ttu-id="22aec-134">字符串</span><span class="sxs-lookup"><span data-stu-id="22aec-134">String</span></span>| <span data-ttu-id="22aec-135">模板的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="22aec-135">Unique identifier for the template.</span></span> <span data-ttu-id="22aec-136">只读。</span><span class="sxs-lookup"><span data-stu-id="22aec-136">Read-only.</span></span>|
|<span data-ttu-id="22aec-137">值</span><span class="sxs-lookup"><span data-stu-id="22aec-137">values</span></span>|<span data-ttu-id="22aec-138">[settingTemplateValue](settingtemplatevalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="22aec-138">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="22aec-139">settemplatevalues 的集合, 该集合列出了组成此模板的可用设置、默认值和类型的集合。</span><span class="sxs-lookup"><span data-stu-id="22aec-139">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="22aec-140">关系</span><span class="sxs-lookup"><span data-stu-id="22aec-140">Relationships</span></span>

<span data-ttu-id="22aec-141">无。</span><span class="sxs-lookup"><span data-stu-id="22aec-141">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="22aec-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="22aec-142">JSON representation</span></span>

<span data-ttu-id="22aec-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22aec-143">Here is a JSON representation of the resource.</span></span>

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
