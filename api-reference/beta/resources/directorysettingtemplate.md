---
title: directorySettingTemplate 资源类型
description: 目录设置模板表示可供租户使用的系统定义设置。 可以基于可用的 directorySettingTemplates 创建目录设置，并将值更改为其预设默认值。 无法创建、更新或删除目录设置模板。 这些设置可以表示租户范围的设置，也可以表示特定的实体设置。  目前，仅有的可用模板适用于 Office 组，并包含诸如用户是否可以创建组或邀请来自组织外部的来宾以成为组成员的设置。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f1881c697eae6b4032635d2e4797a14ef2e848e2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42506461"
---
# <a name="directorysettingtemplate-resource-type"></a><span data-ttu-id="2a8d0-107">directorySettingTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="2a8d0-107">directorySettingTemplate resource type</span></span>

<span data-ttu-id="2a8d0-108">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="2a8d0-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a8d0-109">目录设置模板表示可供租户使用的系统定义设置。</span><span class="sxs-lookup"><span data-stu-id="2a8d0-109">Directory setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="2a8d0-110">可以基于可用的 directorySettingTemplates 创建[目录设置](directorysetting.md)，并将值更改为其预设默认值。</span><span class="sxs-lookup"><span data-stu-id="2a8d0-110">[Directory settings](directorysetting.md) can be created based on the available directorySettingTemplates, and values changed from their preset defaults.</span></span> <span data-ttu-id="2a8d0-111">无法创建、更新或删除目录设置模板。</span><span class="sxs-lookup"><span data-stu-id="2a8d0-111">Directory setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="2a8d0-112">这些设置可以表示租户范围的设置，也可以表示特定的实体设置。</span><span class="sxs-lookup"><span data-stu-id="2a8d0-112">These settings can represent tenant-wide settings, or can represent specific entity settings.</span></span>  <span data-ttu-id="2a8d0-113">目前，仅有的可用模板适用于 Office 组，并包含诸如用户是否可以创建组或邀请来自组织外部的来宾以成为组成员的设置。</span><span class="sxs-lookup"><span data-stu-id="2a8d0-113">Currently, the only templates available apply to Office groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

> <span data-ttu-id="2a8d0-114">**注意**： directorySettingTemplate 资源类型的/beta 版本仅适用于组。</span><span class="sxs-lookup"><span data-stu-id="2a8d0-114">**Note**: The /beta version of the directorySettingTemplate resource type only applies to groups.</span></span> <span data-ttu-id="2a8d0-115">/V1.0 版本已重命名为 groupSettingTemplate。</span><span class="sxs-lookup"><span data-stu-id="2a8d0-115">The /v1.0 version has been renamed to groupSettingTemplate.</span></span>

## <a name="methods"></a><span data-ttu-id="2a8d0-116">方法</span><span class="sxs-lookup"><span data-stu-id="2a8d0-116">Methods</span></span>

| <span data-ttu-id="2a8d0-117">方法</span><span class="sxs-lookup"><span data-stu-id="2a8d0-117">Method</span></span>           | <span data-ttu-id="2a8d0-118">返回类型</span><span class="sxs-lookup"><span data-stu-id="2a8d0-118">Return Type</span></span>    |<span data-ttu-id="2a8d0-119">说明</span><span class="sxs-lookup"><span data-stu-id="2a8d0-119">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2a8d0-120">获取 directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="2a8d0-120">Get directorySettingTemplate</span></span>](../api/directorysettingtemplate-get.md) | [<span data-ttu-id="2a8d0-121">directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="2a8d0-121">directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="2a8d0-122">读取某个系统定义的 directorySettingTemplate 对象的特定属性。</span><span class="sxs-lookup"><span data-stu-id="2a8d0-122">Read the specific properties of one of the system defined directorySettingTemplate objects.</span></span>|
|[<span data-ttu-id="2a8d0-123">列出 directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="2a8d0-123">List directorySettingTemplate</span></span>](../api/directorysettingtemplate-list.md) | [<span data-ttu-id="2a8d0-124">DirectorySettingTemplate 的集合</span><span class="sxs-lookup"><span data-stu-id="2a8d0-124">Collection of directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="2a8d0-125">列出所有系统定义的 directorySettingTemplate 对象。</span><span class="sxs-lookup"><span data-stu-id="2a8d0-125">List all of the system defined directorySettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="2a8d0-126">属性</span><span class="sxs-lookup"><span data-stu-id="2a8d0-126">Properties</span></span>
| <span data-ttu-id="2a8d0-127">属性</span><span class="sxs-lookup"><span data-stu-id="2a8d0-127">Property</span></span>     | <span data-ttu-id="2a8d0-128">类型</span><span class="sxs-lookup"><span data-stu-id="2a8d0-128">Type</span></span>   |<span data-ttu-id="2a8d0-129">说明</span><span class="sxs-lookup"><span data-stu-id="2a8d0-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a8d0-130">说明</span><span class="sxs-lookup"><span data-stu-id="2a8d0-130">description</span></span>|<span data-ttu-id="2a8d0-131">string</span><span class="sxs-lookup"><span data-stu-id="2a8d0-131">string</span></span>|<span data-ttu-id="2a8d0-132">模板的说明。</span><span class="sxs-lookup"><span data-stu-id="2a8d0-132">Description of the template.</span></span> <span data-ttu-id="2a8d0-133">只读。</span><span class="sxs-lookup"><span data-stu-id="2a8d0-133">Read-only.</span></span>|
|<span data-ttu-id="2a8d0-134">displayName</span><span class="sxs-lookup"><span data-stu-id="2a8d0-134">displayName</span></span>|<span data-ttu-id="2a8d0-135">string</span><span class="sxs-lookup"><span data-stu-id="2a8d0-135">string</span></span>|<span data-ttu-id="2a8d0-136">模板的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2a8d0-136">Display name of the template.</span></span> <span data-ttu-id="2a8d0-137">只读。</span><span class="sxs-lookup"><span data-stu-id="2a8d0-137">Read-only.</span></span> |
|<span data-ttu-id="2a8d0-138">id</span><span class="sxs-lookup"><span data-stu-id="2a8d0-138">id</span></span>|<span data-ttu-id="2a8d0-139">字符串</span><span class="sxs-lookup"><span data-stu-id="2a8d0-139">string</span></span>| <span data-ttu-id="2a8d0-140">模板的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2a8d0-140">Unique identifier for the template.</span></span> <span data-ttu-id="2a8d0-141">只读。</span><span class="sxs-lookup"><span data-stu-id="2a8d0-141">Read-only.</span></span>|
|<span data-ttu-id="2a8d0-142">values</span><span class="sxs-lookup"><span data-stu-id="2a8d0-142">values</span></span>|<span data-ttu-id="2a8d0-143">[settingTemplateValue](settingtemplatevalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="2a8d0-143">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="2a8d0-144">Settemplatevalues 的集合，该集合列出了组成此模板的可用设置、默认值和类型的集合。</span><span class="sxs-lookup"><span data-stu-id="2a8d0-144">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span>  <span data-ttu-id="2a8d0-145">只读。</span><span class="sxs-lookup"><span data-stu-id="2a8d0-145">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2a8d0-146">关系</span><span class="sxs-lookup"><span data-stu-id="2a8d0-146">Relationships</span></span>
<span data-ttu-id="2a8d0-147">无</span><span class="sxs-lookup"><span data-stu-id="2a8d0-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="2a8d0-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2a8d0-148">JSON representation</span></span>

<span data-ttu-id="2a8d0-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a8d0-149">Here is a JSON representation of the resource.</span></span>

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
