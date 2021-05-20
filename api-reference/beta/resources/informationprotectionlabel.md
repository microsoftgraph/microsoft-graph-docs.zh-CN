---
title: informationProtectionLabel 资源类型
description: 介绍了信息保护标签，详细介绍了如何向信息正确应用敏感度标签。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: ee8865b4fa898a91ca79cfba29c928ed00e21ae2
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579667"
---
# <a name="informationprotectionlabel-resource-type"></a><span data-ttu-id="63563-103">informationProtectionLabel 资源类型</span><span class="sxs-lookup"><span data-stu-id="63563-103">informationProtectionLabel resource type</span></span>

<span data-ttu-id="63563-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63563-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63563-105">介绍了信息保护标签，详细介绍了如何向信息正确应用敏感度标签。</span><span class="sxs-lookup"><span data-stu-id="63563-105">Describes the information protection label that details how to properly apply a sensitivity label to information.</span></span> <span data-ttu-id="63563-106">**informationProtectionLabel** 资源描述适用于用户或租户的敏感度标签的配置。</span><span class="sxs-lookup"><span data-stu-id="63563-106">The **informationProtectionLabel** resource describes the configuration of sensitivity labels that apply to a user or tenant.</span></span>  

## <a name="methods"></a><span data-ttu-id="63563-107">方法</span><span class="sxs-lookup"><span data-stu-id="63563-107">Methods</span></span>

| <span data-ttu-id="63563-108">方法</span><span class="sxs-lookup"><span data-stu-id="63563-108">Method</span></span>                                                                                              | <span data-ttu-id="63563-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="63563-109">Return Type</span></span>                                                               | <span data-ttu-id="63563-110">说明</span><span class="sxs-lookup"><span data-stu-id="63563-110">Description</span></span>                                                                                                                                                            |
| :-------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------ | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="63563-111">列出 informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="63563-111">List informationProtectionLabel</span></span>](../api/informationprotectionpolicy-list-labels.md)                | <span data-ttu-id="63563-112">[informationProtectionLabel](informationprotectionlabel.md) 集合</span><span class="sxs-lookup"><span data-stu-id="63563-112">[informationProtectionLabel](informationprotectionlabel.md) collection</span></span> | <span data-ttu-id="63563-113">列出用户或租户的所有配置的信息保护标签。</span><span class="sxs-lookup"><span data-stu-id="63563-113">List all configured information protection labels for a user or tenant.</span></span>                                                                                                |
| [<span data-ttu-id="63563-114">获取 informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="63563-114">Get informationProtectionLabel</span></span>](../api/informationprotectionlabel-get.md)                          | [<span data-ttu-id="63563-115">informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="63563-115">informationProtectionLabel</span></span>](informationprotectionlabel.md)               | <span data-ttu-id="63563-116">给定特定标签 ID，返回 **informationProtectionLabel**。</span><span class="sxs-lookup"><span data-stu-id="63563-116">Given a specific label ID, return the **informationProtectionLabel**.</span></span>                                                                                                  |
| [<span data-ttu-id="63563-117">evaluateapplication</span><span class="sxs-lookup"><span data-stu-id="63563-117">evaluateapplication</span></span>](../api/informationprotectionlabel-evaluateapplication.md)                     | <span data-ttu-id="63563-118">[informationProtectionAction](informationprotectionaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="63563-118">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="63563-119">在给定 [contentInfo 和](contentinfo.md) [labelingOptions](labelingoptions.md)的输入后，计算应用标签需要的操作集。</span><span class="sxs-lookup"><span data-stu-id="63563-119">Given an input of [contentInfo](contentinfo.md) and [labelingOptions](labelingoptions.md), compute the set of actions require to apply the label.</span></span>                      |
| [<span data-ttu-id="63563-120">evaluateClassificationResults</span><span class="sxs-lookup"><span data-stu-id="63563-120">evaluateClassificationResults</span></span>](../api/informationprotectionlabel-evaluateclassificationresults.md) | <span data-ttu-id="63563-121">[informationProtectionAction](informationprotectionaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="63563-121">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="63563-122">给定 [contentInfo 的输入](contentinfo.md) 和分类结果，请计算应用标签需要的操作集。</span><span class="sxs-lookup"><span data-stu-id="63563-122">Given an input of [contentInfo](contentinfo.md) and classification results, compute the set of actions require to apply the label.</span></span>                                  |
| [<span data-ttu-id="63563-123">evaluateRemoval</span><span class="sxs-lookup"><span data-stu-id="63563-123">evaluateRemoval</span></span>](../api/informationprotectionlabel-evaluateremoval.md)                             | <span data-ttu-id="63563-124">[informationProtectionAction](informationprotectionaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="63563-124">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="63563-125">在给定 [contentInfo 和](contentinfo.md) [downgradeJustification](downgradejustification.md)的输入后，计算删除标签应采取的操作。</span><span class="sxs-lookup"><span data-stu-id="63563-125">Given an input of [contentInfo](contentinfo.md) and [downgradeJustification](downgradejustification.md), compute the actions that should be taken to remove the label.</span></span> |
| [<span data-ttu-id="63563-126">extractLabel</span><span class="sxs-lookup"><span data-stu-id="63563-126">extractLabel</span></span>](../api/informationprotectionlabel-extractlabel.md)                                   | [<span data-ttu-id="63563-127">informationProtectionContentLabel</span><span class="sxs-lookup"><span data-stu-id="63563-127">informationProtectionContentLabel</span></span>](informationprotectioncontentlabel.md) | <span data-ttu-id="63563-128">在给定 [contentInfo 的输入](contentinfo.md)后，返回元数据表示 [的信息ProtectionLabel](informationprotectionlabel.md) 的详细信息。</span><span class="sxs-lookup"><span data-stu-id="63563-128">Given an input of [contentInfo](contentinfo.md), return details on the [informationProtectionLabel](informationprotectionlabel.md) that the metadata represents.</span></span>       |

## <a name="properties"></a><span data-ttu-id="63563-129">属性</span><span class="sxs-lookup"><span data-stu-id="63563-129">Properties</span></span>

| <span data-ttu-id="63563-130">属性</span><span class="sxs-lookup"><span data-stu-id="63563-130">Property</span></span>    | <span data-ttu-id="63563-131">类型</span><span class="sxs-lookup"><span data-stu-id="63563-131">Type</span></span>    | <span data-ttu-id="63563-132">说明</span><span class="sxs-lookup"><span data-stu-id="63563-132">Description</span></span>                                                                                     |
| :---------- | :------ | :---------------------------------------------------------------------------------------------- |
| <span data-ttu-id="63563-133">color</span><span class="sxs-lookup"><span data-stu-id="63563-133">color</span></span>       | <span data-ttu-id="63563-134">String</span><span class="sxs-lookup"><span data-stu-id="63563-134">String</span></span>  | <span data-ttu-id="63563-135">UI 应为标签显示的颜色（如果已配置）。</span><span class="sxs-lookup"><span data-stu-id="63563-135">The color that the UI should display for the label, if configured.</span></span>                              |
| <span data-ttu-id="63563-136">说明</span><span class="sxs-lookup"><span data-stu-id="63563-136">description</span></span> | <span data-ttu-id="63563-137">String</span><span class="sxs-lookup"><span data-stu-id="63563-137">String</span></span>  | <span data-ttu-id="63563-138">管理员定义的标签说明。</span><span class="sxs-lookup"><span data-stu-id="63563-138">The admin-defined description for the label.</span></span>                                                    |
| <span data-ttu-id="63563-139">id</span><span class="sxs-lookup"><span data-stu-id="63563-139">id</span></span>          | <span data-ttu-id="63563-140">String</span><span class="sxs-lookup"><span data-stu-id="63563-140">String</span></span>  | <span data-ttu-id="63563-141">标签 ID 是 GUID (全局唯) </span><span class="sxs-lookup"><span data-stu-id="63563-141">The label ID is a globally unique identifier (GUID)</span></span>                                             |
| <span data-ttu-id="63563-142">isActive</span><span class="sxs-lookup"><span data-stu-id="63563-142">isActive</span></span>    | <span data-ttu-id="63563-143">布尔</span><span class="sxs-lookup"><span data-stu-id="63563-143">Boolean</span></span> | <span data-ttu-id="63563-144">指示标签是否处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="63563-144">Indicates whether the label is active or not.</span></span> <span data-ttu-id="63563-145">应在 UI 中隐藏或禁用活动标签。</span><span class="sxs-lookup"><span data-stu-id="63563-145">Active labels should be hidden or disabled in UI.</span></span> |
| <span data-ttu-id="63563-146">name</span><span class="sxs-lookup"><span data-stu-id="63563-146">name</span></span>        | <span data-ttu-id="63563-147">String</span><span class="sxs-lookup"><span data-stu-id="63563-147">String</span></span>  | <span data-ttu-id="63563-148">标签的纯文本名称。</span><span class="sxs-lookup"><span data-stu-id="63563-148">The plaintext name of the label.</span></span>                                                                |
| <span data-ttu-id="63563-149">sensitivity</span><span class="sxs-lookup"><span data-stu-id="63563-149">sensitivity</span></span> | <span data-ttu-id="63563-150">Int32</span><span class="sxs-lookup"><span data-stu-id="63563-150">Int32</span></span>   | <span data-ttu-id="63563-151">标签的敏感度值，其中 lower 不太敏感。</span><span class="sxs-lookup"><span data-stu-id="63563-151">The sensitivity value of the label, where lower is less sensitive.</span></span>                              |
| <span data-ttu-id="63563-152">tooltip</span><span class="sxs-lookup"><span data-stu-id="63563-152">tooltip</span></span>     | <span data-ttu-id="63563-153">String</span><span class="sxs-lookup"><span data-stu-id="63563-153">String</span></span>  | <span data-ttu-id="63563-154">应为 UI 中的标签显示的工具提示。</span><span class="sxs-lookup"><span data-stu-id="63563-154">The tooltip that should be displayed for the label in a UI.</span></span>                                     |
| <span data-ttu-id="63563-155">父级</span><span class="sxs-lookup"><span data-stu-id="63563-155">parent</span></span>      | <span data-ttu-id="63563-156">labelDetails</span><span class="sxs-lookup"><span data-stu-id="63563-156">labelDetails</span></span>   | <span data-ttu-id="63563-157">与子标签关联的父标签。</span><span class="sxs-lookup"><span data-stu-id="63563-157">The parent label associated with a child label.</span></span> <span data-ttu-id="63563-158">如果 label 没有父级，则为空。</span><span class="sxs-lookup"><span data-stu-id="63563-158">Null if label has no parent.</span></span>

## <a name="relationships"></a><span data-ttu-id="63563-159">关系</span><span class="sxs-lookup"><span data-stu-id="63563-159">Relationships</span></span>

<span data-ttu-id="63563-160">无。</span><span class="sxs-lookup"><span data-stu-id="63563-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="63563-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="63563-161">JSON representation</span></span>

<span data-ttu-id="63563-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63563-162">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.informationProtectionLabel",
  "keyProperty": "id"
}-->

```json
{
  "color": "String",
  "description": "String",
  "id": "String (identifier)",
  "isActive": true,
  "name": "String",
  "sensitivity": 1024,
  "tooltip": "String",
  "parent": {"@odata.type": "microsoft.graph.labelDetails" }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationProtectionLabel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


