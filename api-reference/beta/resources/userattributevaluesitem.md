---
title: userAttributeValuesItem 资源类型
description: 用于在用户流中有多个选项可供选择时填充用户流属性的值。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 64b2416cd6fd0e8c92d9a00ff2d599226e3cd02c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133019"
---
# <a name="userattributevaluesitem-resource-type"></a><span data-ttu-id="da19f-103">userAttributeValuesItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="da19f-103">userAttributeValuesItem resource type</span></span>

<span data-ttu-id="da19f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da19f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="da19f-105">用于在用户流中有多个选项可供选择时填充用户流属性的值。</span><span class="sxs-lookup"><span data-stu-id="da19f-105">Used to populate the values for a user flow attribute within a user flow when there are multiple selections to choose from.</span></span> <span data-ttu-id="da19f-106">userAttributeValuesItem 适用于 userInputTypes `radioSingleSelect` `dropdownSingleSelect` 和 `checkboxMultiSelect` [identityUserFlowAttributeAssignment。](..\resources\identityuserflowattributeassignment.md)</span><span class="sxs-lookup"><span data-stu-id="da19f-106">userAttributeValuesItem is applicable to the userInputTypes `radioSingleSelect`, `dropdownSingleSelect`, and `checkboxMultiSelect` for an [identityUserFlowAttributeAssignment](..\resources\identityuserflowattributeassignment.md).</span></span>

## <a name="properties"></a><span data-ttu-id="da19f-107">属性</span><span class="sxs-lookup"><span data-stu-id="da19f-107">Properties</span></span>

|<span data-ttu-id="da19f-108">属性</span><span class="sxs-lookup"><span data-stu-id="da19f-108">Property</span></span>|<span data-ttu-id="da19f-109">类型</span><span class="sxs-lookup"><span data-stu-id="da19f-109">Type</span></span>|<span data-ttu-id="da19f-110">说明</span><span class="sxs-lookup"><span data-stu-id="da19f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da19f-111">isDefault</span><span class="sxs-lookup"><span data-stu-id="da19f-111">isDefault</span></span>|<span data-ttu-id="da19f-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="da19f-112">Boolean</span></span>|<span data-ttu-id="da19f-113">用于将值设置为默认值。</span><span class="sxs-lookup"><span data-stu-id="da19f-113">Used to set the value as the default.</span></span>|
|<span data-ttu-id="da19f-114">name</span><span class="sxs-lookup"><span data-stu-id="da19f-114">name</span></span>|<span data-ttu-id="da19f-115">字符串</span><span class="sxs-lookup"><span data-stu-id="da19f-115">String</span></span>|<span data-ttu-id="da19f-116">在显示名称流中向最终用户显示的属性的列表。</span><span class="sxs-lookup"><span data-stu-id="da19f-116">The display name of the property displayed to the end user in the user flow.</span></span>|
|<span data-ttu-id="da19f-117">value</span><span class="sxs-lookup"><span data-stu-id="da19f-117">value</span></span>|<span data-ttu-id="da19f-118">String</span><span class="sxs-lookup"><span data-stu-id="da19f-118">String</span></span>|<span data-ttu-id="da19f-119">选择此项时设置的值。</span><span class="sxs-lookup"><span data-stu-id="da19f-119">The value that is set when this item is selected.</span></span>|

## <a name="relationships"></a><span data-ttu-id="da19f-120">关系</span><span class="sxs-lookup"><span data-stu-id="da19f-120">Relationships</span></span>

<span data-ttu-id="da19f-121">无。</span><span class="sxs-lookup"><span data-stu-id="da19f-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="da19f-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="da19f-122">JSON representation</span></span>

<span data-ttu-id="da19f-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da19f-123">The following is a JSON representation of the resource.</span></span>
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
