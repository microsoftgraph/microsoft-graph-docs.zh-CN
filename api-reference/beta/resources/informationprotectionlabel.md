---
title: informationProtectionLabel 资源类型
description: 介绍信息保护标签，这些标签详细说明了如何正确地将敏感标签应用于信息。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 528238d904ac9807027dd51a8c59ed03570c7bc3
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938742"
---
# <a name="informationprotectionlabel-resource-type"></a><span data-ttu-id="9328a-103">informationProtectionLabel 资源类型</span><span class="sxs-lookup"><span data-stu-id="9328a-103">informationProtectionLabel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9328a-104">介绍信息保护标签，这些标签详细说明了如何正确地将敏感标签应用于信息。</span><span class="sxs-lookup"><span data-stu-id="9328a-104">Describes the information protection label that details how to properly apply a sensitivity label to information.</span></span> <span data-ttu-id="9328a-105">**InformationProtectionLabel**资源描述了适用于用户或租户的敏感度标签的配置。</span><span class="sxs-lookup"><span data-stu-id="9328a-105">The **informationProtectionLabel** resource describes the configuration of sensitivity labels that apply to a user or tenant.</span></span>  

## <a name="methods"></a><span data-ttu-id="9328a-106">方法</span><span class="sxs-lookup"><span data-stu-id="9328a-106">Methods</span></span>

| <span data-ttu-id="9328a-107">方法</span><span class="sxs-lookup"><span data-stu-id="9328a-107">Method</span></span>                                                                                              | <span data-ttu-id="9328a-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="9328a-108">Return Type</span></span>                                                               | <span data-ttu-id="9328a-109">说明</span><span class="sxs-lookup"><span data-stu-id="9328a-109">Description</span></span>                                                                                                                                                            |
| :-------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------ | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="9328a-110">列出 informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="9328a-110">List informationProtectionLabel</span></span>](../api/informationprotectionpolicy-list-labels.md)                | <span data-ttu-id="9328a-111">[informationProtectionLabel](informationprotectionlabel.md)集合</span><span class="sxs-lookup"><span data-stu-id="9328a-111">[informationProtectionLabel](informationprotectionlabel.md) collection</span></span> | <span data-ttu-id="9328a-112">列出用户或租户的所有已配置的信息保护标签。</span><span class="sxs-lookup"><span data-stu-id="9328a-112">List all configured information protection labels for a user or tenant.</span></span>                                                                                                |
| [<span data-ttu-id="9328a-113">获取 informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="9328a-113">Get informationProtectionLabel</span></span>](../api/informationprotectionlabel-get.md)                          | [<span data-ttu-id="9328a-114">informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="9328a-114">informationProtectionLabel</span></span>](informationprotectionlabel.md)               | <span data-ttu-id="9328a-115">在给定特定标签 ID 的情况下，返回**informationProtectionLabel**。</span><span class="sxs-lookup"><span data-stu-id="9328a-115">Given a specific label ID, return the **informationProtectionLabel**.</span></span>                                                                                                  |
| [<span data-ttu-id="9328a-116">evaluateapplication</span><span class="sxs-lookup"><span data-stu-id="9328a-116">evaluateapplication</span></span>](../api/informationprotectionlabel-evaluateapplication.md)                     | <span data-ttu-id="9328a-117">[informationProtectionAction](informationprotectionaction.md)集合</span><span class="sxs-lookup"><span data-stu-id="9328a-117">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="9328a-118">给定[contentInfo](contentinfo.md)和[labelingOptions](labelingoptions.md)的输入，计算一组操作需要应用标签。</span><span class="sxs-lookup"><span data-stu-id="9328a-118">Given an input of [contentInfo](contentinfo.md) and [labelingOptions](labelingoptions.md), compute the set of actions require to apply the label.</span></span>                      |
| [<span data-ttu-id="9328a-119">evaluateClassificationResults</span><span class="sxs-lookup"><span data-stu-id="9328a-119">evaluateClassificationResults</span></span>](../api/informationprotectionlabel-evaluateclassificationresults.md) | <span data-ttu-id="9328a-120">[informationProtectionAction](informationprotectionaction.md)集合</span><span class="sxs-lookup"><span data-stu-id="9328a-120">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="9328a-121">给定[contentInfo](contentinfo.md)和分类结果的输入，计算一组操作需要应用标签。</span><span class="sxs-lookup"><span data-stu-id="9328a-121">Given an input of [contentInfo](contentinfo.md) and classification results, compute the set of actions require to apply the label.</span></span>                                  |
| [<span data-ttu-id="9328a-122">evaluateRemoval</span><span class="sxs-lookup"><span data-stu-id="9328a-122">evaluateRemoval</span></span>](../api/informationprotectionlabel-evaluateremoval.md)                             | <span data-ttu-id="9328a-123">[informationProtectionAction](informationprotectionaction.md)集合</span><span class="sxs-lookup"><span data-stu-id="9328a-123">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="9328a-124">给定[contentInfo](contentinfo.md)和[downgradeJustification](downgradejustification.md)的输入，计算要删除标签应采取的操作。</span><span class="sxs-lookup"><span data-stu-id="9328a-124">Given an input of [contentInfo](contentinfo.md) and [downgradeJustification](downgradejustification.md), compute the actions that should be taken to remove the label.</span></span> |
| [<span data-ttu-id="9328a-125">extractLabel</span><span class="sxs-lookup"><span data-stu-id="9328a-125">extractLabel</span></span>](../api/informationprotectionlabel-extractlabel.md)                                   | [<span data-ttu-id="9328a-126">informationProtectionContentLabel</span><span class="sxs-lookup"><span data-stu-id="9328a-126">informationProtectionContentLabel</span></span>](informationprotectioncontentlabel.md) | <span data-ttu-id="9328a-127">给定[contentInfo](contentinfo.md)的输入，返回有关元数据表示的[informationProtectionLabel](informationprotectionlabel.md)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="9328a-127">Given an input of [contentInfo](contentinfo.md), return details on the [informationProtectionLabel](informationprotectionlabel.md) that the metadata represents.</span></span>       |

## <a name="properties"></a><span data-ttu-id="9328a-128">属性</span><span class="sxs-lookup"><span data-stu-id="9328a-128">Properties</span></span>

| <span data-ttu-id="9328a-129">属性</span><span class="sxs-lookup"><span data-stu-id="9328a-129">Property</span></span>    | <span data-ttu-id="9328a-130">类型</span><span class="sxs-lookup"><span data-stu-id="9328a-130">Type</span></span>    | <span data-ttu-id="9328a-131">描述</span><span class="sxs-lookup"><span data-stu-id="9328a-131">Description</span></span>                                                                                     |
| :---------- | :------ | :---------------------------------------------------------------------------------------------- |
| <span data-ttu-id="9328a-132">color</span><span class="sxs-lookup"><span data-stu-id="9328a-132">color</span></span>       | <span data-ttu-id="9328a-133">String</span><span class="sxs-lookup"><span data-stu-id="9328a-133">String</span></span>  | <span data-ttu-id="9328a-134">UI 应为标签显示的颜色（如果已配置）。</span><span class="sxs-lookup"><span data-stu-id="9328a-134">The color that the UI should display for the label, if configured.</span></span>                              |
| <span data-ttu-id="9328a-135">description</span><span class="sxs-lookup"><span data-stu-id="9328a-135">description</span></span> | <span data-ttu-id="9328a-136">String</span><span class="sxs-lookup"><span data-stu-id="9328a-136">String</span></span>  | <span data-ttu-id="9328a-137">管理员定义的标签说明。</span><span class="sxs-lookup"><span data-stu-id="9328a-137">The admin-defined description for the label.</span></span>                                                    |
| <span data-ttu-id="9328a-138">id</span><span class="sxs-lookup"><span data-stu-id="9328a-138">id</span></span>          | <span data-ttu-id="9328a-139">String</span><span class="sxs-lookup"><span data-stu-id="9328a-139">String</span></span>  | <span data-ttu-id="9328a-140">标签 ID 是一个全局唯一标识符（GUID）</span><span class="sxs-lookup"><span data-stu-id="9328a-140">The label ID is a globally unique identifier (GUID)</span></span>                                             |
| <span data-ttu-id="9328a-141">isActive</span><span class="sxs-lookup"><span data-stu-id="9328a-141">isActive</span></span>    | <span data-ttu-id="9328a-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="9328a-142">Boolean</span></span> | <span data-ttu-id="9328a-143">指示标签是否处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="9328a-143">Indicates whether the label is active or not.</span></span> <span data-ttu-id="9328a-144">应在 UI 中隐藏或禁用活动标签。</span><span class="sxs-lookup"><span data-stu-id="9328a-144">Active labels should be hidden or disabled in UI.</span></span> |
| <span data-ttu-id="9328a-145">name</span><span class="sxs-lookup"><span data-stu-id="9328a-145">name</span></span>        | <span data-ttu-id="9328a-146">字符串</span><span class="sxs-lookup"><span data-stu-id="9328a-146">String</span></span>  | <span data-ttu-id="9328a-147">标签的纯文本名称。</span><span class="sxs-lookup"><span data-stu-id="9328a-147">The plaintext name of the label.</span></span>                                                                |
| <span data-ttu-id="9328a-148">sensitivity</span><span class="sxs-lookup"><span data-stu-id="9328a-148">sensitivity</span></span> | <span data-ttu-id="9328a-149">Int32</span><span class="sxs-lookup"><span data-stu-id="9328a-149">Int32</span></span>   | <span data-ttu-id="9328a-150">标签的敏感度值，其中较小的是不敏感的。</span><span class="sxs-lookup"><span data-stu-id="9328a-150">The sensitivity value of the label, where lower is less sensitive.</span></span>                              |
| <span data-ttu-id="9328a-151">tooltip</span><span class="sxs-lookup"><span data-stu-id="9328a-151">tooltip</span></span>     | <span data-ttu-id="9328a-152">字符串</span><span class="sxs-lookup"><span data-stu-id="9328a-152">String</span></span>  | <span data-ttu-id="9328a-153">应为 UI 中的标签显示的工具提示。</span><span class="sxs-lookup"><span data-stu-id="9328a-153">The tooltip that should be displayed for the label in a UI.</span></span>                                     |

## <a name="relationships"></a><span data-ttu-id="9328a-154">关系</span><span class="sxs-lookup"><span data-stu-id="9328a-154">Relationships</span></span>

<span data-ttu-id="9328a-155">无。</span><span class="sxs-lookup"><span data-stu-id="9328a-155">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9328a-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9328a-156">JSON representation</span></span>

<span data-ttu-id="9328a-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9328a-157">The following is a JSON representation of the resource.</span></span>

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
