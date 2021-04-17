---
title: userAttributeValuesItem 资源类型
description: 表示用户流中的用户流属性值。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 367f5d835f3790c589a8d7d28b7994484fd9613c
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882396"
---
# <a name="userattributevaluesitem-resource-type"></a><span data-ttu-id="cf61b-103">userAttributeValuesItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="cf61b-103">userAttributeValuesItem resource type</span></span>

<span data-ttu-id="cf61b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf61b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cf61b-105">表示用户流中的用户流属性值，当有多个选择可供选择时。</span><span class="sxs-lookup"><span data-stu-id="cf61b-105">Represents user flow attribute values within a user flow when there are multiple selections to choose from.</span></span>  <span data-ttu-id="cf61b-106">userAttributeValuesItem 适用于 、 和 的 userInputTypes，适用于 `radioSingleSelect` `dropdownSingleSelect` `checkboxMultiSelect` [identityUserFlowAttributeAssignment](..\resources\identityuserflowattributeassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="cf61b-106">The userAttributeValuesItem is applicable to the userInputTypes of `radioSingleSelect`, `dropdownSingleSelect`, and `checkboxMultiSelect` for an [identityUserFlowAttributeAssignment](..\resources\identityuserflowattributeassignment.md).</span></span>

## <a name="properties"></a><span data-ttu-id="cf61b-107">属性</span><span class="sxs-lookup"><span data-stu-id="cf61b-107">Properties</span></span>

|<span data-ttu-id="cf61b-108">属性</span><span class="sxs-lookup"><span data-stu-id="cf61b-108">Property</span></span>|<span data-ttu-id="cf61b-109">类型</span><span class="sxs-lookup"><span data-stu-id="cf61b-109">Type</span></span>|<span data-ttu-id="cf61b-110">说明</span><span class="sxs-lookup"><span data-stu-id="cf61b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf61b-111">isDefault</span><span class="sxs-lookup"><span data-stu-id="cf61b-111">isDefault</span></span>|<span data-ttu-id="cf61b-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf61b-112">Boolean</span></span>|<span data-ttu-id="cf61b-113">确定是否将该值设置为默认值。</span><span class="sxs-lookup"><span data-stu-id="cf61b-113">Determines whether the value is set as the default.</span></span>|
|<span data-ttu-id="cf61b-114">name</span><span class="sxs-lookup"><span data-stu-id="cf61b-114">name</span></span>|<span data-ttu-id="cf61b-115">String</span><span class="sxs-lookup"><span data-stu-id="cf61b-115">String</span></span>|<span data-ttu-id="cf61b-116">在显示名称流中向用户显示的属性的行数。</span><span class="sxs-lookup"><span data-stu-id="cf61b-116">The display name of the property displayed to the user in the user flow.</span></span>|
|<span data-ttu-id="cf61b-117">value</span><span class="sxs-lookup"><span data-stu-id="cf61b-117">value</span></span>|<span data-ttu-id="cf61b-118">String</span><span class="sxs-lookup"><span data-stu-id="cf61b-118">String</span></span>|<span data-ttu-id="cf61b-119">选择此项时设置的值。</span><span class="sxs-lookup"><span data-stu-id="cf61b-119">The value that is set when this item is selected.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf61b-120">关系</span><span class="sxs-lookup"><span data-stu-id="cf61b-120">Relationships</span></span>

<span data-ttu-id="cf61b-121">无。</span><span class="sxs-lookup"><span data-stu-id="cf61b-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cf61b-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cf61b-122">JSON representation</span></span>

<span data-ttu-id="cf61b-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf61b-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userAttributeValuesItem"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userAttributeValuesItem",
  "name": "String",
  "value": "String",
  "isDefault": "Boolean"
}
```
