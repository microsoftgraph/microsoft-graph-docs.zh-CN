---
title: userAttributeValuesItem 资源类型
description: 当有多个选择可供选择时，用于填充用户流中用户流属性的值。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6fd0d582ef4dcdd83dba6947536c5acdbc14a8cb
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581323"
---
# <a name="userattributevaluesitem-resource-type"></a><span data-ttu-id="ced40-103">userAttributeValuesItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="ced40-103">userAttributeValuesItem resource type</span></span>

<span data-ttu-id="ced40-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ced40-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ced40-105">当有多个选择可供选择时，用于填充用户流中用户流属性的值。</span><span class="sxs-lookup"><span data-stu-id="ced40-105">Used to populate the values for a user flow attribute within a user flow when there are multiple selections to choose from.</span></span> <span data-ttu-id="ced40-106">userAttributeValuesItem 适用于 userInputTypes `radioSingleSelect` 、 `dropdownSingleSelect` 和 `checkboxMultiSelect` [identityUserFlowAttributeAssignment](..\resources\identityuserflowattributeassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="ced40-106">userAttributeValuesItem is applicable to the userInputTypes `radioSingleSelect`, `dropdownSingleSelect`, and `checkboxMultiSelect` for an [identityUserFlowAttributeAssignment](..\resources\identityuserflowattributeassignment.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ced40-107">属性</span><span class="sxs-lookup"><span data-stu-id="ced40-107">Properties</span></span>

|<span data-ttu-id="ced40-108">属性</span><span class="sxs-lookup"><span data-stu-id="ced40-108">Property</span></span>|<span data-ttu-id="ced40-109">类型</span><span class="sxs-lookup"><span data-stu-id="ced40-109">Type</span></span>|<span data-ttu-id="ced40-110">Description</span><span class="sxs-lookup"><span data-stu-id="ced40-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ced40-111">isDefault</span><span class="sxs-lookup"><span data-stu-id="ced40-111">isDefault</span></span>|<span data-ttu-id="ced40-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="ced40-112">Boolean</span></span>|<span data-ttu-id="ced40-113">用于将值设置为默认值。</span><span class="sxs-lookup"><span data-stu-id="ced40-113">Used to set the value as the default.</span></span>|
|<span data-ttu-id="ced40-114">name</span><span class="sxs-lookup"><span data-stu-id="ced40-114">name</span></span>|<span data-ttu-id="ced40-115">String</span><span class="sxs-lookup"><span data-stu-id="ced40-115">String</span></span>|<span data-ttu-id="ced40-116">在用户流中向最终用户显示的属性的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ced40-116">The display name of the property displayed to the end user in the user flow.</span></span>|
|<span data-ttu-id="ced40-117">value</span><span class="sxs-lookup"><span data-stu-id="ced40-117">value</span></span>|<span data-ttu-id="ced40-118">String</span><span class="sxs-lookup"><span data-stu-id="ced40-118">String</span></span>|<span data-ttu-id="ced40-119">选择此项时设置的值。</span><span class="sxs-lookup"><span data-stu-id="ced40-119">The value that is set when this item is selected.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ced40-120">关系</span><span class="sxs-lookup"><span data-stu-id="ced40-120">Relationships</span></span>

<span data-ttu-id="ced40-121">无。</span><span class="sxs-lookup"><span data-stu-id="ced40-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ced40-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ced40-122">JSON representation</span></span>

<span data-ttu-id="ced40-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ced40-123">The following is a JSON representation of the resource.</span></span>
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
