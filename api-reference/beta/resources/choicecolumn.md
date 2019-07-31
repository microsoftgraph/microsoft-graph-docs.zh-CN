---
author: JeremyKelley
description: columnDefinition 资源上的 choiceColumn 指示可从所选列表中选择列的值。
ms.date: 09/11/2017
title: ChoiceColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 72ef8adb96614fc32b9aee8141eb19248e963639
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973486"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="85939-103">ChoiceColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="85939-103">ChoiceColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85939-104">[columnDefinition](columndefinition.md) 资源上的 **choiceColumn** 指示可从所选列表中选择列的值。</span><span class="sxs-lookup"><span data-stu-id="85939-104">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="85939-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="85939-105">JSON representation</span></span>

<span data-ttu-id="85939-106">下面是 **choiceColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85939-106">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="85939-107">属性</span><span class="sxs-lookup"><span data-stu-id="85939-107">Properties</span></span>

| <span data-ttu-id="85939-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="85939-108">Property name</span></span>      | <span data-ttu-id="85939-109">类型</span><span class="sxs-lookup"><span data-stu-id="85939-109">Type</span></span>               | <span data-ttu-id="85939-110">说明</span><span class="sxs-lookup"><span data-stu-id="85939-110">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="85939-111">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="85939-111">**allowTextEntry**</span></span> | <span data-ttu-id="85939-112">boolean</span><span class="sxs-lookup"><span data-stu-id="85939-112">boolean</span></span>            | <span data-ttu-id="85939-113">如果为 true，则允许配置选择之外的自定义值。</span><span class="sxs-lookup"><span data-stu-id="85939-113">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="85939-114">**choices**</span><span class="sxs-lookup"><span data-stu-id="85939-114">**choices**</span></span>        | <span data-ttu-id="85939-115">collection(string)</span><span class="sxs-lookup"><span data-stu-id="85939-115">collection(string)</span></span> | <span data-ttu-id="85939-116">可用于此列的值列表。</span><span class="sxs-lookup"><span data-stu-id="85939-116">The list of values available for this column.</span></span>
| <span data-ttu-id="85939-117">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="85939-117">**displayAs**</span></span>      | <span data-ttu-id="85939-118">string</span><span class="sxs-lookup"><span data-stu-id="85939-118">string</span></span>             | <span data-ttu-id="85939-119">选择在用户体验中的显示方式。</span><span class="sxs-lookup"><span data-stu-id="85939-119">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="85939-120">必须为 `checkBoxes`、`dropDownMenu` 或 `radioButtons` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="85939-120">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn",
  "suppressions": []
}
-->
