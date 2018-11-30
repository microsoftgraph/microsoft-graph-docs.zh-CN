---
title: directorySettingTemplate 资源类型
description: 系统定义供租户的设置表示目录设置模板。 目录设置可以创建基于可用 directorySettingTemplates 和更改的预设默认值。 无法创建、 更新或删除目录设置模板。 这些设置可表示租户范围的设置，或可表示特定实体设置。  目前，唯一可用的模板适用于 Office 的组，并包括设置如用户可以创建组还是邀请来宾从组织外部成为组的成员。
ms.openlocfilehash: fa4906aa58805e6d1a027973f61b5d68ed47f2c1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041773"
---
# <a name="directorysettingtemplate-resource-type"></a><span data-ttu-id="afb64-107">directorySettingTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="afb64-107">directorySettingTemplate resource type</span></span>

> <span data-ttu-id="afb64-108">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="afb64-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="afb64-109">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="afb64-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="afb64-110">系统定义供租户的设置表示目录设置模板。</span><span class="sxs-lookup"><span data-stu-id="afb64-110">Directory setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="afb64-111">[目录设置](directorysetting.md)可以创建基于可用 directorySettingTemplates 和更改的预设默认值。</span><span class="sxs-lookup"><span data-stu-id="afb64-111">[Directory settings](directorysetting.md) can be created based on the available directorySettingTemplates, and values changed from their preset defaults.</span></span> <span data-ttu-id="afb64-112">无法创建、 更新或删除目录设置模板。</span><span class="sxs-lookup"><span data-stu-id="afb64-112">Directory setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="afb64-113">这些设置可表示租户范围的设置，或可表示特定实体设置。</span><span class="sxs-lookup"><span data-stu-id="afb64-113">These settings can represent tenant-wide settings, or can represent specific entity settings.</span></span>  <span data-ttu-id="afb64-114">目前，唯一可用的模板适用于 Office 的组，并包括设置如用户可以创建组还是邀请来宾从组织外部成为组的成员。</span><span class="sxs-lookup"><span data-stu-id="afb64-114">Currently, the only templates available apply to Office groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

> <span data-ttu-id="afb64-115">**注意**： directorySettingTemplate 资源类型的 /beta 版本仅适用于组。</span><span class="sxs-lookup"><span data-stu-id="afb64-115">**Note**: The /beta version of the directorySettingTemplate resource type only applies to groups.</span></span> <span data-ttu-id="afb64-116">/V1.0 版本已被重命名为 groupSettingTemplate。</span><span class="sxs-lookup"><span data-stu-id="afb64-116">The /v1.0 version has been renamed to groupSettingTemplate.</span></span>

## <a name="methods"></a><span data-ttu-id="afb64-117">方法</span><span class="sxs-lookup"><span data-stu-id="afb64-117">Methods</span></span>

| <span data-ttu-id="afb64-118">方法</span><span class="sxs-lookup"><span data-stu-id="afb64-118">Method</span></span>           | <span data-ttu-id="afb64-119">返回类型</span><span class="sxs-lookup"><span data-stu-id="afb64-119">Return Type</span></span>    |<span data-ttu-id="afb64-120">说明</span><span class="sxs-lookup"><span data-stu-id="afb64-120">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="afb64-121">获取 directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="afb64-121">Get directorySettingTemplate</span></span>](../api/directorysettingtemplate-get.md) | [<span data-ttu-id="afb64-122">directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="afb64-122">directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="afb64-123">读取的一个系统定义 directorySettingTemplate 对象的特定属性。</span><span class="sxs-lookup"><span data-stu-id="afb64-123">Read the specific properties of one of the system defined directorySettingTemplate objects.</span></span>|
|[<span data-ttu-id="afb64-124">列表 directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="afb64-124">List directorySettingTemplate</span></span>](../api/directorysettingtemplate-list.md) | [<span data-ttu-id="afb64-125">DirectorySettingTemplate 的集合</span><span class="sxs-lookup"><span data-stu-id="afb64-125">Collection of directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="afb64-126">列出的所有系统定义 directorySettingTemplate 对象。</span><span class="sxs-lookup"><span data-stu-id="afb64-126">List all of the system defined directorySettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="afb64-127">属性</span><span class="sxs-lookup"><span data-stu-id="afb64-127">Properties</span></span>
| <span data-ttu-id="afb64-128">属性</span><span class="sxs-lookup"><span data-stu-id="afb64-128">Property</span></span>     | <span data-ttu-id="afb64-129">类型</span><span class="sxs-lookup"><span data-stu-id="afb64-129">Type</span></span>   |<span data-ttu-id="afb64-130">说明</span><span class="sxs-lookup"><span data-stu-id="afb64-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="afb64-131">说明</span><span class="sxs-lookup"><span data-stu-id="afb64-131">description</span></span>|<span data-ttu-id="afb64-132">string</span><span class="sxs-lookup"><span data-stu-id="afb64-132">string</span></span>|<span data-ttu-id="afb64-133">模板描述</span><span class="sxs-lookup"><span data-stu-id="afb64-133">Description of the template.</span></span> <span data-ttu-id="afb64-134">只读。</span><span class="sxs-lookup"><span data-stu-id="afb64-134">Read-only.</span></span>|
|<span data-ttu-id="afb64-135">displayName</span><span class="sxs-lookup"><span data-stu-id="afb64-135">displayName</span></span>|<span data-ttu-id="afb64-136">string</span><span class="sxs-lookup"><span data-stu-id="afb64-136">string</span></span>|<span data-ttu-id="afb64-137">模板的显示名称</span><span class="sxs-lookup"><span data-stu-id="afb64-137">Display name of the template.</span></span> <span data-ttu-id="afb64-138">只读。</span><span class="sxs-lookup"><span data-stu-id="afb64-138">Read-only.</span></span> |
|<span data-ttu-id="afb64-139">id</span><span class="sxs-lookup"><span data-stu-id="afb64-139">id</span></span>|<span data-ttu-id="afb64-140">string</span><span class="sxs-lookup"><span data-stu-id="afb64-140">string</span></span>| <span data-ttu-id="afb64-p107">模板的的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="afb64-p107">Unique identifier for the template. Read-only.</span></span>|
|<span data-ttu-id="afb64-143">values</span><span class="sxs-lookup"><span data-stu-id="afb64-143">values</span></span>|<span data-ttu-id="afb64-144">[settingTemplateValue](settingtemplatevalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="afb64-144">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="afb64-145">setTemplateValues 的集合，列出组成此模板的一组可用设置、默认值和类型。</span><span class="sxs-lookup"><span data-stu-id="afb64-145">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span>  <span data-ttu-id="afb64-146">只读。</span><span class="sxs-lookup"><span data-stu-id="afb64-146">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="afb64-147">Relationships</span><span class="sxs-lookup"><span data-stu-id="afb64-147">Relationships</span></span>
<span data-ttu-id="afb64-148">无</span><span class="sxs-lookup"><span data-stu-id="afb64-148">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="afb64-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="afb64-149">JSON representation</span></span>

<span data-ttu-id="afb64-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="afb64-150">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "directorySettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->