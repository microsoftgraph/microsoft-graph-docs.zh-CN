---
title: informationProtectionLabel 资源类型
description: 介绍信息保护标签，这些标签详细说明了如何正确地将敏感标签应用于信息。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 183a5856aafd8aa2a5b8b1fe3b1eb48bddcc5358
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496038"
---
# <a name="informationprotectionlabel-resource-type"></a><span data-ttu-id="99d0a-103">informationProtectionLabel 资源类型</span><span class="sxs-lookup"><span data-stu-id="99d0a-103">informationProtectionLabel resource type</span></span>

<span data-ttu-id="99d0a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="99d0a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99d0a-105">介绍信息保护标签，这些标签详细说明了如何正确地将敏感标签应用于信息。</span><span class="sxs-lookup"><span data-stu-id="99d0a-105">Describes the information protection label that details how to properly apply a sensitivity label to information.</span></span> <span data-ttu-id="99d0a-106">**InformationProtectionLabel**资源描述了适用于用户或租户的敏感度标签的配置。</span><span class="sxs-lookup"><span data-stu-id="99d0a-106">The **informationProtectionLabel** resource describes the configuration of sensitivity labels that apply to a user or tenant.</span></span>  

## <a name="methods"></a><span data-ttu-id="99d0a-107">方法</span><span class="sxs-lookup"><span data-stu-id="99d0a-107">Methods</span></span>

| <span data-ttu-id="99d0a-108">方法</span><span class="sxs-lookup"><span data-stu-id="99d0a-108">Method</span></span>                                                                                              | <span data-ttu-id="99d0a-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="99d0a-109">Return Type</span></span>                                                               | <span data-ttu-id="99d0a-110">说明</span><span class="sxs-lookup"><span data-stu-id="99d0a-110">Description</span></span>                                                                                                                                                            |
| :-------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------ | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="99d0a-111">列出 informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="99d0a-111">List informationProtectionLabel</span></span>](../api/informationprotectionpolicy-list-labels.md)                | <span data-ttu-id="99d0a-112">[informationProtectionLabel](informationprotectionlabel.md)集合</span><span class="sxs-lookup"><span data-stu-id="99d0a-112">[informationProtectionLabel](informationprotectionlabel.md) collection</span></span> | <span data-ttu-id="99d0a-113">列出用户或租户的所有已配置的信息保护标签。</span><span class="sxs-lookup"><span data-stu-id="99d0a-113">List all configured information protection labels for a user or tenant.</span></span>                                                                                                |
| [<span data-ttu-id="99d0a-114">获取 informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="99d0a-114">Get informationProtectionLabel</span></span>](../api/informationprotectionlabel-get.md)                          | [<span data-ttu-id="99d0a-115">informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="99d0a-115">informationProtectionLabel</span></span>](informationprotectionlabel.md)               | <span data-ttu-id="99d0a-116">在给定特定标签 ID 的情况下，返回**informationProtectionLabel**。</span><span class="sxs-lookup"><span data-stu-id="99d0a-116">Given a specific label ID, return the **informationProtectionLabel**.</span></span>                                                                                                  |
| [<span data-ttu-id="99d0a-117">evaluateapplication</span><span class="sxs-lookup"><span data-stu-id="99d0a-117">evaluateapplication</span></span>](../api/informationprotectionlabel-evaluateapplication.md)                     | <span data-ttu-id="99d0a-118">[informationProtectionAction](informationprotectionaction.md)集合</span><span class="sxs-lookup"><span data-stu-id="99d0a-118">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="99d0a-119">给定[contentInfo](contentinfo.md)和[labelingOptions](labelingoptions.md)的输入，计算一组操作需要应用标签。</span><span class="sxs-lookup"><span data-stu-id="99d0a-119">Given an input of [contentInfo](contentinfo.md) and [labelingOptions](labelingoptions.md), compute the set of actions require to apply the label.</span></span>                      |
| [<span data-ttu-id="99d0a-120">evaluateClassificationResults</span><span class="sxs-lookup"><span data-stu-id="99d0a-120">evaluateClassificationResults</span></span>](../api/informationprotectionlabel-evaluateclassificationresults.md) | <span data-ttu-id="99d0a-121">[informationProtectionAction](informationprotectionaction.md)集合</span><span class="sxs-lookup"><span data-stu-id="99d0a-121">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="99d0a-122">给定[contentInfo](contentinfo.md)和分类结果的输入，计算一组操作需要应用标签。</span><span class="sxs-lookup"><span data-stu-id="99d0a-122">Given an input of [contentInfo](contentinfo.md) and classification results, compute the set of actions require to apply the label.</span></span>                                  |
| [<span data-ttu-id="99d0a-123">evaluateRemoval</span><span class="sxs-lookup"><span data-stu-id="99d0a-123">evaluateRemoval</span></span>](../api/informationprotectionlabel-evaluateremoval.md)                             | <span data-ttu-id="99d0a-124">[informationProtectionAction](informationprotectionaction.md)集合</span><span class="sxs-lookup"><span data-stu-id="99d0a-124">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="99d0a-125">给定[contentInfo](contentinfo.md)和[downgradeJustification](downgradejustification.md)的输入，计算要删除标签应采取的操作。</span><span class="sxs-lookup"><span data-stu-id="99d0a-125">Given an input of [contentInfo](contentinfo.md) and [downgradeJustification](downgradejustification.md), compute the actions that should be taken to remove the label.</span></span> |
| [<span data-ttu-id="99d0a-126">extractLabel</span><span class="sxs-lookup"><span data-stu-id="99d0a-126">extractLabel</span></span>](../api/informationprotectionlabel-extractlabel.md)                                   | [<span data-ttu-id="99d0a-127">informationProtectionContentLabel</span><span class="sxs-lookup"><span data-stu-id="99d0a-127">informationProtectionContentLabel</span></span>](informationprotectioncontentlabel.md) | <span data-ttu-id="99d0a-128">给定[contentInfo](contentinfo.md)的输入，返回有关元数据表示的[informationProtectionLabel](informationprotectionlabel.md)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="99d0a-128">Given an input of [contentInfo](contentinfo.md), return details on the [informationProtectionLabel](informationprotectionlabel.md) that the metadata represents.</span></span>       |

## <a name="properties"></a><span data-ttu-id="99d0a-129">属性</span><span class="sxs-lookup"><span data-stu-id="99d0a-129">Properties</span></span>

| <span data-ttu-id="99d0a-130">属性</span><span class="sxs-lookup"><span data-stu-id="99d0a-130">Property</span></span>    | <span data-ttu-id="99d0a-131">类型</span><span class="sxs-lookup"><span data-stu-id="99d0a-131">Type</span></span>    | <span data-ttu-id="99d0a-132">说明</span><span class="sxs-lookup"><span data-stu-id="99d0a-132">Description</span></span>                                                                                     |
| :---------- | :------ | :---------------------------------------------------------------------------------------------- |
| <span data-ttu-id="99d0a-133">color</span><span class="sxs-lookup"><span data-stu-id="99d0a-133">color</span></span>       | <span data-ttu-id="99d0a-134">String</span><span class="sxs-lookup"><span data-stu-id="99d0a-134">String</span></span>  | <span data-ttu-id="99d0a-135">UI 应为标签显示的颜色（如果已配置）。</span><span class="sxs-lookup"><span data-stu-id="99d0a-135">The color that the UI should display for the label, if configured.</span></span>                              |
| <span data-ttu-id="99d0a-136">说明</span><span class="sxs-lookup"><span data-stu-id="99d0a-136">description</span></span> | <span data-ttu-id="99d0a-137">String</span><span class="sxs-lookup"><span data-stu-id="99d0a-137">String</span></span>  | <span data-ttu-id="99d0a-138">管理员定义的标签说明。</span><span class="sxs-lookup"><span data-stu-id="99d0a-138">The admin-defined description for the label.</span></span>                                                    |
| <span data-ttu-id="99d0a-139">id</span><span class="sxs-lookup"><span data-stu-id="99d0a-139">id</span></span>          | <span data-ttu-id="99d0a-140">String</span><span class="sxs-lookup"><span data-stu-id="99d0a-140">String</span></span>  | <span data-ttu-id="99d0a-141">标签 ID 是一个全局唯一标识符（GUID）</span><span class="sxs-lookup"><span data-stu-id="99d0a-141">The label ID is a globally unique identifier (GUID)</span></span>                                             |
| <span data-ttu-id="99d0a-142">isActive</span><span class="sxs-lookup"><span data-stu-id="99d0a-142">isActive</span></span>    | <span data-ttu-id="99d0a-143">布尔</span><span class="sxs-lookup"><span data-stu-id="99d0a-143">Boolean</span></span> | <span data-ttu-id="99d0a-144">指示标签是否处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="99d0a-144">Indicates whether the label is active or not.</span></span> <span data-ttu-id="99d0a-145">应在 UI 中隐藏或禁用活动标签。</span><span class="sxs-lookup"><span data-stu-id="99d0a-145">Active labels should be hidden or disabled in UI.</span></span> |
| <span data-ttu-id="99d0a-146">name</span><span class="sxs-lookup"><span data-stu-id="99d0a-146">name</span></span>        | <span data-ttu-id="99d0a-147">字符串</span><span class="sxs-lookup"><span data-stu-id="99d0a-147">String</span></span>  | <span data-ttu-id="99d0a-148">标签的纯文本名称。</span><span class="sxs-lookup"><span data-stu-id="99d0a-148">The plaintext name of the label.</span></span>                                                                |
| <span data-ttu-id="99d0a-149">sensitivity</span><span class="sxs-lookup"><span data-stu-id="99d0a-149">sensitivity</span></span> | <span data-ttu-id="99d0a-150">Int32</span><span class="sxs-lookup"><span data-stu-id="99d0a-150">Int32</span></span>   | <span data-ttu-id="99d0a-151">标签的敏感度值，其中较小的是不敏感的。</span><span class="sxs-lookup"><span data-stu-id="99d0a-151">The sensitivity value of the label, where lower is less sensitive.</span></span>                              |
| <span data-ttu-id="99d0a-152">tooltip</span><span class="sxs-lookup"><span data-stu-id="99d0a-152">tooltip</span></span>     | <span data-ttu-id="99d0a-153">String</span><span class="sxs-lookup"><span data-stu-id="99d0a-153">String</span></span>  | <span data-ttu-id="99d0a-154">应为 UI 中的标签显示的工具提示。</span><span class="sxs-lookup"><span data-stu-id="99d0a-154">The tooltip that should be displayed for the label in a UI.</span></span>                                     |

## <a name="relationships"></a><span data-ttu-id="99d0a-155">关系</span><span class="sxs-lookup"><span data-stu-id="99d0a-155">Relationships</span></span>

<span data-ttu-id="99d0a-156">无。</span><span class="sxs-lookup"><span data-stu-id="99d0a-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="99d0a-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99d0a-157">JSON representation</span></span>

<span data-ttu-id="99d0a-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99d0a-158">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.informationProtectionLabel",
  "baseType": "",
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
