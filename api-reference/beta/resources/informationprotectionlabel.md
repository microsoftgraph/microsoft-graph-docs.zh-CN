---
title: informationProtectionLabel 资源类型
description: 介绍了信息保护标签，详细介绍了如何向信息正确应用敏感度标签。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 4937d428fd480c0f31a5368a76c4eede9efef851
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953753"
---
# <a name="informationprotectionlabel-resource-type"></a><span data-ttu-id="52170-103">informationProtectionLabel 资源类型</span><span class="sxs-lookup"><span data-stu-id="52170-103">informationProtectionLabel resource type</span></span>

<span data-ttu-id="52170-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52170-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52170-105">介绍了信息保护标签，详细介绍了如何向信息正确应用敏感度标签。</span><span class="sxs-lookup"><span data-stu-id="52170-105">Describes the information protection label that details how to properly apply a sensitivity label to information.</span></span> <span data-ttu-id="52170-106">**informationProtectionLabel** 资源描述适用于用户或租户的敏感度标签的配置。</span><span class="sxs-lookup"><span data-stu-id="52170-106">The **informationProtectionLabel** resource describes the configuration of sensitivity labels that apply to a user or tenant.</span></span>  

## <a name="methods"></a><span data-ttu-id="52170-107">Methods</span><span class="sxs-lookup"><span data-stu-id="52170-107">Methods</span></span>

| <span data-ttu-id="52170-108">方法</span><span class="sxs-lookup"><span data-stu-id="52170-108">Method</span></span>                                                                                              | <span data-ttu-id="52170-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="52170-109">Return Type</span></span>                                                               | <span data-ttu-id="52170-110">说明</span><span class="sxs-lookup"><span data-stu-id="52170-110">Description</span></span>                                                                                                                                                            |
| :-------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------ | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="52170-111">列出 informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="52170-111">List informationProtectionLabel</span></span>](../api/informationprotectionpolicy-list-labels.md)                | <span data-ttu-id="52170-112">[informationProtectionLabel](informationprotectionlabel.md) 集合</span><span class="sxs-lookup"><span data-stu-id="52170-112">[informationProtectionLabel](informationprotectionlabel.md) collection</span></span> | <span data-ttu-id="52170-113">列出用户或租户的所有配置的信息保护标签。</span><span class="sxs-lookup"><span data-stu-id="52170-113">List all configured information protection labels for a user or tenant.</span></span>                                                                                                |
| [<span data-ttu-id="52170-114">获取 informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="52170-114">Get informationProtectionLabel</span></span>](../api/informationprotectionlabel-get.md)                          | [<span data-ttu-id="52170-115">informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="52170-115">informationProtectionLabel</span></span>](informationprotectionlabel.md)               | <span data-ttu-id="52170-116">给定特定标签 ID，返回 **informationProtectionLabel**。</span><span class="sxs-lookup"><span data-stu-id="52170-116">Given a specific label ID, return the **informationProtectionLabel**.</span></span>                                                                                                  |
| [<span data-ttu-id="52170-117">evaluateapplication</span><span class="sxs-lookup"><span data-stu-id="52170-117">evaluateapplication</span></span>](../api/informationprotectionlabel-evaluateapplication.md)                     | <span data-ttu-id="52170-118">[informationProtectionAction](informationprotectionaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="52170-118">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="52170-119">在给定 [contentInfo 和](contentinfo.md) [labelingOptions](labelingoptions.md)的输入后，计算应用标签需要的操作集。</span><span class="sxs-lookup"><span data-stu-id="52170-119">Given an input of [contentInfo](contentinfo.md) and [labelingOptions](labelingoptions.md), compute the set of actions require to apply the label.</span></span>                      |
| [<span data-ttu-id="52170-120">evaluateClassificationResults</span><span class="sxs-lookup"><span data-stu-id="52170-120">evaluateClassificationResults</span></span>](../api/informationprotectionlabel-evaluateclassificationresults.md) | <span data-ttu-id="52170-121">[informationProtectionAction](informationprotectionaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="52170-121">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="52170-122">给定 [contentInfo 的输入](contentinfo.md) 和分类结果，请计算应用标签需要的操作集。</span><span class="sxs-lookup"><span data-stu-id="52170-122">Given an input of [contentInfo](contentinfo.md) and classification results, compute the set of actions require to apply the label.</span></span>                                  |
| [<span data-ttu-id="52170-123">evaluateRemoval</span><span class="sxs-lookup"><span data-stu-id="52170-123">evaluateRemoval</span></span>](../api/informationprotectionlabel-evaluateremoval.md)                             | <span data-ttu-id="52170-124">[informationProtectionAction](informationprotectionaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="52170-124">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="52170-125">在给定 [contentInfo 和](contentinfo.md) [downgradeJustification](downgradejustification.md)的输入后，计算删除标签应采取的操作。</span><span class="sxs-lookup"><span data-stu-id="52170-125">Given an input of [contentInfo](contentinfo.md) and [downgradeJustification](downgradejustification.md), compute the actions that should be taken to remove the label.</span></span> |
| [<span data-ttu-id="52170-126">extractLabel</span><span class="sxs-lookup"><span data-stu-id="52170-126">extractLabel</span></span>](../api/informationprotectionlabel-extractlabel.md)                                   | [<span data-ttu-id="52170-127">informationProtectionContentLabel</span><span class="sxs-lookup"><span data-stu-id="52170-127">informationProtectionContentLabel</span></span>](informationprotectioncontentlabel.md) | <span data-ttu-id="52170-128">在给定 [contentInfo 的输入](contentinfo.md)后，返回元数据表示 [的信息ProtectionLabel](informationprotectionlabel.md) 的详细信息。</span><span class="sxs-lookup"><span data-stu-id="52170-128">Given an input of [contentInfo](contentinfo.md), return details on the [informationProtectionLabel](informationprotectionlabel.md) that the metadata represents.</span></span>       |

## <a name="properties"></a><span data-ttu-id="52170-129">属性</span><span class="sxs-lookup"><span data-stu-id="52170-129">Properties</span></span>

| <span data-ttu-id="52170-130">属性</span><span class="sxs-lookup"><span data-stu-id="52170-130">Property</span></span>    | <span data-ttu-id="52170-131">类型</span><span class="sxs-lookup"><span data-stu-id="52170-131">Type</span></span>    | <span data-ttu-id="52170-132">说明</span><span class="sxs-lookup"><span data-stu-id="52170-132">Description</span></span>                                                                                     |
| :---------- | :------ | :---------------------------------------------------------------------------------------------- |
| <span data-ttu-id="52170-133">color</span><span class="sxs-lookup"><span data-stu-id="52170-133">color</span></span>       | <span data-ttu-id="52170-134">String</span><span class="sxs-lookup"><span data-stu-id="52170-134">String</span></span>  | <span data-ttu-id="52170-135">UI 应为标签显示的颜色（如果已配置）。</span><span class="sxs-lookup"><span data-stu-id="52170-135">The color that the UI should display for the label, if configured.</span></span>                              |
| <span data-ttu-id="52170-136">说明</span><span class="sxs-lookup"><span data-stu-id="52170-136">description</span></span> | <span data-ttu-id="52170-137">String</span><span class="sxs-lookup"><span data-stu-id="52170-137">String</span></span>  | <span data-ttu-id="52170-138">管理员定义的标签说明。</span><span class="sxs-lookup"><span data-stu-id="52170-138">The admin-defined description for the label.</span></span>                                                    |
| <span data-ttu-id="52170-139">id</span><span class="sxs-lookup"><span data-stu-id="52170-139">id</span></span>          | <span data-ttu-id="52170-140">String</span><span class="sxs-lookup"><span data-stu-id="52170-140">String</span></span>  | <span data-ttu-id="52170-141">标签 ID 是 GUID (全局唯) </span><span class="sxs-lookup"><span data-stu-id="52170-141">The label ID is a globally unique identifier (GUID)</span></span>                                             |
| <span data-ttu-id="52170-142">isActive</span><span class="sxs-lookup"><span data-stu-id="52170-142">isActive</span></span>    | <span data-ttu-id="52170-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="52170-143">Boolean</span></span> | <span data-ttu-id="52170-144">指示标签是否处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="52170-144">Indicates whether the label is active or not.</span></span> <span data-ttu-id="52170-145">应在 UI 中隐藏或禁用活动标签。</span><span class="sxs-lookup"><span data-stu-id="52170-145">Active labels should be hidden or disabled in UI.</span></span> |
| <span data-ttu-id="52170-146">name</span><span class="sxs-lookup"><span data-stu-id="52170-146">name</span></span>        | <span data-ttu-id="52170-147">String</span><span class="sxs-lookup"><span data-stu-id="52170-147">String</span></span>  | <span data-ttu-id="52170-148">标签的纯文本名称。</span><span class="sxs-lookup"><span data-stu-id="52170-148">The plaintext name of the label.</span></span>                                                                |
| <span data-ttu-id="52170-149">敏感度</span><span class="sxs-lookup"><span data-stu-id="52170-149">sensitivity</span></span> | <span data-ttu-id="52170-150">Int32</span><span class="sxs-lookup"><span data-stu-id="52170-150">Int32</span></span>   | <span data-ttu-id="52170-151">标签的敏感度值，其中 lower 不太敏感。</span><span class="sxs-lookup"><span data-stu-id="52170-151">The sensitivity value of the label, where lower is less sensitive.</span></span>                              |
| <span data-ttu-id="52170-152">tooltip</span><span class="sxs-lookup"><span data-stu-id="52170-152">tooltip</span></span>     | <span data-ttu-id="52170-153">String</span><span class="sxs-lookup"><span data-stu-id="52170-153">String</span></span>  | <span data-ttu-id="52170-154">应为 UI 中的标签显示的工具提示。</span><span class="sxs-lookup"><span data-stu-id="52170-154">The tooltip that should be displayed for the label in a UI.</span></span>                                     |

## <a name="relationships"></a><span data-ttu-id="52170-155">关系</span><span class="sxs-lookup"><span data-stu-id="52170-155">Relationships</span></span>

<span data-ttu-id="52170-156">无。</span><span class="sxs-lookup"><span data-stu-id="52170-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="52170-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="52170-157">JSON representation</span></span>

<span data-ttu-id="52170-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52170-158">The following is a JSON representation of the resource.</span></span>

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
  "tooltip": "String"
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


