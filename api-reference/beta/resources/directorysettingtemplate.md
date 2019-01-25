---
title: directorySettingTemplate 资源类型
description: 系统定义供租户的设置表示目录设置模板。 目录设置可以创建基于可用 directorySettingTemplates 和更改的预设默认值。 无法创建、 更新或删除目录设置模板。 这些设置可表示租户范围的设置，或可表示特定实体设置。  目前，唯一可用的模板适用于 Office 的组，并包括设置如用户可以创建组还是邀请来宾从组织外部成为组的成员。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 366817df422686a8db658f1cab1d5805c24c4f91
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516656"
---
# <a name="directorysettingtemplate-resource-type"></a><span data-ttu-id="6872d-107">directorySettingTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="6872d-107">directorySettingTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6872d-108">系统定义供租户的设置表示目录设置模板。</span><span class="sxs-lookup"><span data-stu-id="6872d-108">Directory setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="6872d-109">[目录设置](directorysetting.md)可以创建基于可用 directorySettingTemplates 和更改的预设默认值。</span><span class="sxs-lookup"><span data-stu-id="6872d-109">[Directory settings](directorysetting.md) can be created based on the available directorySettingTemplates, and values changed from their preset defaults.</span></span> <span data-ttu-id="6872d-110">无法创建、 更新或删除目录设置模板。</span><span class="sxs-lookup"><span data-stu-id="6872d-110">Directory setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="6872d-111">这些设置可表示租户范围的设置，或可表示特定实体设置。</span><span class="sxs-lookup"><span data-stu-id="6872d-111">These settings can represent tenant-wide settings, or can represent specific entity settings.</span></span>  <span data-ttu-id="6872d-112">目前，唯一可用的模板适用于 Office 的组，并包括设置如用户可以创建组还是邀请来宾从组织外部成为组的成员。</span><span class="sxs-lookup"><span data-stu-id="6872d-112">Currently, the only templates available apply to Office groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

> <span data-ttu-id="6872d-113">**注意**： directorySettingTemplate 资源类型的 /beta 版本仅适用于组。</span><span class="sxs-lookup"><span data-stu-id="6872d-113">**Note**: The /beta version of the directorySettingTemplate resource type only applies to groups.</span></span> <span data-ttu-id="6872d-114">/V1.0 版本已被重命名为 groupSettingTemplate。</span><span class="sxs-lookup"><span data-stu-id="6872d-114">The /v1.0 version has been renamed to groupSettingTemplate.</span></span>

## <a name="methods"></a><span data-ttu-id="6872d-115">方法</span><span class="sxs-lookup"><span data-stu-id="6872d-115">Methods</span></span>

| <span data-ttu-id="6872d-116">方法</span><span class="sxs-lookup"><span data-stu-id="6872d-116">Method</span></span>           | <span data-ttu-id="6872d-117">返回类型</span><span class="sxs-lookup"><span data-stu-id="6872d-117">Return Type</span></span>    |<span data-ttu-id="6872d-118">说明</span><span class="sxs-lookup"><span data-stu-id="6872d-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6872d-119">获取 directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="6872d-119">Get directorySettingTemplate</span></span>](../api/directorysettingtemplate-get.md) | [<span data-ttu-id="6872d-120">directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="6872d-120">directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="6872d-121">读取的一个系统定义 directorySettingTemplate 对象的特定属性。</span><span class="sxs-lookup"><span data-stu-id="6872d-121">Read the specific properties of one of the system defined directorySettingTemplate objects.</span></span>|
|[<span data-ttu-id="6872d-122">列表 directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="6872d-122">List directorySettingTemplate</span></span>](../api/directorysettingtemplate-list.md) | [<span data-ttu-id="6872d-123">DirectorySettingTemplate 的集合</span><span class="sxs-lookup"><span data-stu-id="6872d-123">Collection of directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="6872d-124">列出的所有系统定义 directorySettingTemplate 对象。</span><span class="sxs-lookup"><span data-stu-id="6872d-124">List all of the system defined directorySettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="6872d-125">属性</span><span class="sxs-lookup"><span data-stu-id="6872d-125">Properties</span></span>
| <span data-ttu-id="6872d-126">属性</span><span class="sxs-lookup"><span data-stu-id="6872d-126">Property</span></span>     | <span data-ttu-id="6872d-127">类型</span><span class="sxs-lookup"><span data-stu-id="6872d-127">Type</span></span>   |<span data-ttu-id="6872d-128">说明</span><span class="sxs-lookup"><span data-stu-id="6872d-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6872d-129">description</span><span class="sxs-lookup"><span data-stu-id="6872d-129">description</span></span>|<span data-ttu-id="6872d-130">string</span><span class="sxs-lookup"><span data-stu-id="6872d-130">string</span></span>|<span data-ttu-id="6872d-131">模板描述</span><span class="sxs-lookup"><span data-stu-id="6872d-131">Description of the template.</span></span> <span data-ttu-id="6872d-132">只读。</span><span class="sxs-lookup"><span data-stu-id="6872d-132">Read-only.</span></span>|
|<span data-ttu-id="6872d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="6872d-133">displayName</span></span>|<span data-ttu-id="6872d-134">string</span><span class="sxs-lookup"><span data-stu-id="6872d-134">string</span></span>|<span data-ttu-id="6872d-135">模板的显示名称</span><span class="sxs-lookup"><span data-stu-id="6872d-135">Display name of the template.</span></span> <span data-ttu-id="6872d-136">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="6872d-136">Read-only.</span></span> |
|<span data-ttu-id="6872d-137">id</span><span class="sxs-lookup"><span data-stu-id="6872d-137">id</span></span>|<span data-ttu-id="6872d-138">string</span><span class="sxs-lookup"><span data-stu-id="6872d-138">string</span></span>| <span data-ttu-id="6872d-p106">模板的的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="6872d-p106">Unique identifier for the template. Read-only.</span></span>|
|<span data-ttu-id="6872d-141">values</span><span class="sxs-lookup"><span data-stu-id="6872d-141">values</span></span>|<span data-ttu-id="6872d-142">[settingTemplateValue](settingtemplatevalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6872d-142">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="6872d-143">setTemplateValues 的集合，列出组成此模板的一组可用设置、默认值和类型。</span><span class="sxs-lookup"><span data-stu-id="6872d-143">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span>  <span data-ttu-id="6872d-144">只读。</span><span class="sxs-lookup"><span data-stu-id="6872d-144">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6872d-145">关系</span><span class="sxs-lookup"><span data-stu-id="6872d-145">Relationships</span></span>
<span data-ttu-id="6872d-146">无</span><span class="sxs-lookup"><span data-stu-id="6872d-146">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6872d-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6872d-147">JSON representation</span></span>

<span data-ttu-id="6872d-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6872d-148">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/directorysettingtemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
