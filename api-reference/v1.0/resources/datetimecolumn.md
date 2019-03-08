---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: DateTimeColumn
localization_priority: Normal
ms.openlocfilehash: ba650ccbe307ba286cf2182bda35a21f3c675114
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480171"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="50f15-102">DateTimeColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="50f15-102">DateTimeColumn resource type</span></span>

<span data-ttu-id="50f15-103">[columnDefinition](columndefinition.md) 资源上的 **dateTimeColumn** 指示该列的值为日期或时间。</span><span class="sxs-lookup"><span data-stu-id="50f15-103">The **dateTimeColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="50f15-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="50f15-104">JSON representation</span></span>

<span data-ttu-id="50f15-105">下面是 **dateTimeColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50f15-105">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="50f15-106">属性</span><span class="sxs-lookup"><span data-stu-id="50f15-106">Properties</span></span>

| <span data-ttu-id="50f15-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="50f15-107">Property name</span></span>      | <span data-ttu-id="50f15-108">类型</span><span class="sxs-lookup"><span data-stu-id="50f15-108">Type</span></span>               | <span data-ttu-id="50f15-109">说明</span><span class="sxs-lookup"><span data-stu-id="50f15-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="50f15-110">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="50f15-110">**displayAs**</span></span>      | <span data-ttu-id="50f15-111">string</span><span class="sxs-lookup"><span data-stu-id="50f15-111">string</span></span>             | <span data-ttu-id="50f15-112">值在用户体验中的显示方式。</span><span class="sxs-lookup"><span data-stu-id="50f15-112">How the value should be presented in the UX.</span></span> <span data-ttu-id="50f15-113">必须为 `default`、`friendly` 或 `standard` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="50f15-113">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="50f15-114">有关详细信息，请参阅下文。</span><span class="sxs-lookup"><span data-stu-id="50f15-114">See below for more details.</span></span> <span data-ttu-id="50f15-115">如果未指定，则视为 `default`。</span><span class="sxs-lookup"><span data-stu-id="50f15-115">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="50f15-116">**format**</span><span class="sxs-lookup"><span data-stu-id="50f15-116">**format**</span></span>         | <span data-ttu-id="50f15-117">string</span><span class="sxs-lookup"><span data-stu-id="50f15-117">string</span></span>             | <span data-ttu-id="50f15-118">指示值是否应该只显示为日期或日期和时间。</span><span class="sxs-lookup"><span data-stu-id="50f15-118">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="50f15-119">必须为 `dateOnly` 或 `dateTime` 的其中一个</span><span class="sxs-lookup"><span data-stu-id="50f15-119">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-options"></a><span data-ttu-id="50f15-120">DisplayAs 选项</span><span class="sxs-lookup"><span data-stu-id="50f15-120">DisplayAs options</span></span>

| <span data-ttu-id="50f15-121">值</span><span class="sxs-lookup"><span data-stu-id="50f15-121">Value</span></span>        | <span data-ttu-id="50f15-122">说明</span><span class="sxs-lookup"><span data-stu-id="50f15-122">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="50f15-123">**default**</span><span class="sxs-lookup"><span data-stu-id="50f15-123">**default**</span></span>  | <span data-ttu-id="50f15-124">使用用户体验中呈现的默认值。</span><span class="sxs-lookup"><span data-stu-id="50f15-124">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="50f15-125">**friendly**</span><span class="sxs-lookup"><span data-stu-id="50f15-125">**friendly**</span></span> | <span data-ttu-id="50f15-126">使用友好相对表示形式（如</span><span class="sxs-lookup"><span data-stu-id="50f15-126">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="50f15-127">“今天下午 3:00”）</span><span class="sxs-lookup"><span data-stu-id="50f15-127">"today at 3:00 PM")</span></span>
| <span data-ttu-id="50f15-128">**standard**</span><span class="sxs-lookup"><span data-stu-id="50f15-128">**standard**</span></span> | <span data-ttu-id="50f15-129">使用标准绝对表示形式（如</span><span class="sxs-lookup"><span data-stu-id="50f15-129">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="50f15-130">“2017 年 5 月 10 日下午 3:20”）</span><span class="sxs-lookup"><span data-stu-id="50f15-130">"5/10/2017 3:20 PM")</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/choicecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(checkBoxes,dropDownMenu,radioButtons) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/datetimecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(default,friendly,standard) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/datetimecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(dateOnly,dateTime) are in resource, but () are in table"
  ],
  "tocPath": "Resources/DateTimeColumn"
} -->
