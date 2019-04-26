---
title: directorySettingTemplate 资源类型
description: 目录设置模板表示可供租户使用的系统定义设置。 可以基于可用的 directorySettingTemplates 创建目录设置, 并将值更改为其预设默认值。 无法创建、更新或删除目录设置模板。 这些设置可以表示租户范围的设置, 也可以表示特定的实体设置。  目前, 仅有的可用模板适用于 Office 组, 并包含诸如用户是否可以创建组或邀请来自组织外部的来宾以成为组成员的设置。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 73109edd383fe6f7d705f86f707c2096f8d9ac58
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340747"
---
# <a name="directorysettingtemplate-resource-type"></a><span data-ttu-id="fb273-107">directorySettingTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="fb273-107">directorySettingTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb273-108">目录设置模板表示可供租户使用的系统定义设置。</span><span class="sxs-lookup"><span data-stu-id="fb273-108">Directory setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="fb273-109">可以基于可用的 directorySettingTemplates 创建[目录设置](directorysetting.md), 并将值更改为其预设默认值。</span><span class="sxs-lookup"><span data-stu-id="fb273-109">[Directory settings](directorysetting.md) can be created based on the available directorySettingTemplates, and values changed from their preset defaults.</span></span> <span data-ttu-id="fb273-110">无法创建、更新或删除目录设置模板。</span><span class="sxs-lookup"><span data-stu-id="fb273-110">Directory setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="fb273-111">这些设置可以表示租户范围的设置, 也可以表示特定的实体设置。</span><span class="sxs-lookup"><span data-stu-id="fb273-111">These settings can represent tenant-wide settings, or can represent specific entity settings.</span></span>  <span data-ttu-id="fb273-112">目前, 仅有的可用模板适用于 Office 组, 并包含诸如用户是否可以创建组或邀请来自组织外部的来宾以成为组成员的设置。</span><span class="sxs-lookup"><span data-stu-id="fb273-112">Currently, the only templates available apply to Office groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

> <span data-ttu-id="fb273-113">**注意**: directorySettingTemplate 资源类型的/beta 版本仅适用于组。</span><span class="sxs-lookup"><span data-stu-id="fb273-113">**Note**: The /beta version of the directorySettingTemplate resource type only applies to groups.</span></span> <span data-ttu-id="fb273-114">/v1.0 版本已重命名为 groupSettingTemplate。</span><span class="sxs-lookup"><span data-stu-id="fb273-114">The /v1.0 version has been renamed to groupSettingTemplate.</span></span>

## <a name="methods"></a><span data-ttu-id="fb273-115">方法</span><span class="sxs-lookup"><span data-stu-id="fb273-115">Methods</span></span>

| <span data-ttu-id="fb273-116">方法</span><span class="sxs-lookup"><span data-stu-id="fb273-116">Method</span></span>           | <span data-ttu-id="fb273-117">返回类型</span><span class="sxs-lookup"><span data-stu-id="fb273-117">Return Type</span></span>    |<span data-ttu-id="fb273-118">说明</span><span class="sxs-lookup"><span data-stu-id="fb273-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fb273-119">获取 directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="fb273-119">Get directorySettingTemplate</span></span>](../api/directorysettingtemplate-get.md) | [<span data-ttu-id="fb273-120">directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="fb273-120">directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="fb273-121">读取某个系统定义的 directorySettingTemplate 对象的特定属性。</span><span class="sxs-lookup"><span data-stu-id="fb273-121">Read the specific properties of one of the system defined directorySettingTemplate objects.</span></span>|
|[<span data-ttu-id="fb273-122">列出 directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="fb273-122">List directorySettingTemplate</span></span>](../api/directorysettingtemplate-list.md) | [<span data-ttu-id="fb273-123">directorySettingTemplate 的集合</span><span class="sxs-lookup"><span data-stu-id="fb273-123">Collection of directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="fb273-124">列出所有系统定义的 directorySettingTemplate 对象。</span><span class="sxs-lookup"><span data-stu-id="fb273-124">List all of the system defined directorySettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="fb273-125">属性</span><span class="sxs-lookup"><span data-stu-id="fb273-125">Properties</span></span>
| <span data-ttu-id="fb273-126">属性</span><span class="sxs-lookup"><span data-stu-id="fb273-126">Property</span></span>     | <span data-ttu-id="fb273-127">类型</span><span class="sxs-lookup"><span data-stu-id="fb273-127">Type</span></span>   |<span data-ttu-id="fb273-128">说明</span><span class="sxs-lookup"><span data-stu-id="fb273-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb273-129">说明</span><span class="sxs-lookup"><span data-stu-id="fb273-129">description</span></span>|<span data-ttu-id="fb273-130">string</span><span class="sxs-lookup"><span data-stu-id="fb273-130">string</span></span>|<span data-ttu-id="fb273-131">模板的说明。</span><span class="sxs-lookup"><span data-stu-id="fb273-131">Description of the template.</span></span> <span data-ttu-id="fb273-132">只读。</span><span class="sxs-lookup"><span data-stu-id="fb273-132">Read-only.</span></span>|
|<span data-ttu-id="fb273-133">displayName</span><span class="sxs-lookup"><span data-stu-id="fb273-133">displayName</span></span>|<span data-ttu-id="fb273-134">string</span><span class="sxs-lookup"><span data-stu-id="fb273-134">string</span></span>|<span data-ttu-id="fb273-135">模板的显示名称。</span><span class="sxs-lookup"><span data-stu-id="fb273-135">Display name of the template.</span></span> <span data-ttu-id="fb273-136">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="fb273-136">Read-only.</span></span> |
|<span data-ttu-id="fb273-137">id</span><span class="sxs-lookup"><span data-stu-id="fb273-137">id</span></span>|<span data-ttu-id="fb273-138">字符串</span><span class="sxs-lookup"><span data-stu-id="fb273-138">string</span></span>| <span data-ttu-id="fb273-139">模板的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="fb273-139">Unique identifier for the template.</span></span> <span data-ttu-id="fb273-140">只读。</span><span class="sxs-lookup"><span data-stu-id="fb273-140">Read-only.</span></span>|
|<span data-ttu-id="fb273-141">values</span><span class="sxs-lookup"><span data-stu-id="fb273-141">values</span></span>|<span data-ttu-id="fb273-142">[settingTemplateValue](settingtemplatevalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="fb273-142">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="fb273-143">settemplatevalues 的集合, 该集合列出了组成此模板的可用设置、默认值和类型的集合。</span><span class="sxs-lookup"><span data-stu-id="fb273-143">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span>  <span data-ttu-id="fb273-144">只读。</span><span class="sxs-lookup"><span data-stu-id="fb273-144">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="fb273-145">关系</span><span class="sxs-lookup"><span data-stu-id="fb273-145">Relationships</span></span>
<span data-ttu-id="fb273-146">无</span><span class="sxs-lookup"><span data-stu-id="fb273-146">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="fb273-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fb273-147">JSON representation</span></span>

<span data-ttu-id="fb273-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb273-148">Here is a JSON representation of the resource.</span></span>

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
