---
author: JeremyKelley
ms.date: 09/11/2017
title: DateTimeColumn
localization_priority: Normal
description: columnDefinition 资源上的 dateTimeColumn 指示该列的值为日期或时间。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 28639277416b4bcea3caf641413078e355ff9de7
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239644"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="190d0-103">DateTimeColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="190d0-103">DateTimeColumn resource type</span></span>

<span data-ttu-id="190d0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="190d0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="190d0-105">[columnDefinition](columndefinition.md) 资源上的 **dateTimeColumn** 指示该列的值为日期或时间。</span><span class="sxs-lookup"><span data-stu-id="190d0-105">The **dateTimeColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="190d0-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="190d0-106">JSON representation</span></span>

<span data-ttu-id="190d0-107">下面是 **dateTimeColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="190d0-107">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="190d0-108">属性</span><span class="sxs-lookup"><span data-stu-id="190d0-108">Properties</span></span>

| <span data-ttu-id="190d0-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="190d0-109">Property name</span></span>      | <span data-ttu-id="190d0-110">类型</span><span class="sxs-lookup"><span data-stu-id="190d0-110">Type</span></span>               | <span data-ttu-id="190d0-111">说明</span><span class="sxs-lookup"><span data-stu-id="190d0-111">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="190d0-112">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="190d0-112">**displayAs**</span></span>      | <span data-ttu-id="190d0-113">string</span><span class="sxs-lookup"><span data-stu-id="190d0-113">string</span></span>             | <span data-ttu-id="190d0-114">值在用户体验中的显示方式。</span><span class="sxs-lookup"><span data-stu-id="190d0-114">How the value should be presented in the UX.</span></span> <span data-ttu-id="190d0-115">必须为 `default`、`friendly` 或 `standard` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="190d0-115">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="190d0-116">有关详细信息，请参阅下文。</span><span class="sxs-lookup"><span data-stu-id="190d0-116">See below for more details.</span></span> <span data-ttu-id="190d0-117">如果未指定，则视为 `default`。</span><span class="sxs-lookup"><span data-stu-id="190d0-117">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="190d0-118">**format**</span><span class="sxs-lookup"><span data-stu-id="190d0-118">**format**</span></span>         | <span data-ttu-id="190d0-119">string</span><span class="sxs-lookup"><span data-stu-id="190d0-119">string</span></span>             | <span data-ttu-id="190d0-120">指示值是否应该只显示为日期或日期和时间。</span><span class="sxs-lookup"><span data-stu-id="190d0-120">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="190d0-121">必须为 `dateOnly` 或 `dateTime` 的其中一个</span><span class="sxs-lookup"><span data-stu-id="190d0-121">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-options"></a><span data-ttu-id="190d0-122">DisplayAs 选项</span><span class="sxs-lookup"><span data-stu-id="190d0-122">DisplayAs options</span></span>

| <span data-ttu-id="190d0-123">值</span><span class="sxs-lookup"><span data-stu-id="190d0-123">Value</span></span>        | <span data-ttu-id="190d0-124">说明</span><span class="sxs-lookup"><span data-stu-id="190d0-124">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="190d0-125">**default**</span><span class="sxs-lookup"><span data-stu-id="190d0-125">**default**</span></span>  | <span data-ttu-id="190d0-126">使用用户体验中呈现的默认值。</span><span class="sxs-lookup"><span data-stu-id="190d0-126">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="190d0-127">**friendly**</span><span class="sxs-lookup"><span data-stu-id="190d0-127">**friendly**</span></span> | <span data-ttu-id="190d0-128">使用友好相对表示形式（如</span><span class="sxs-lookup"><span data-stu-id="190d0-128">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="190d0-129">“今天下午 3:00”）</span><span class="sxs-lookup"><span data-stu-id="190d0-129">"today at 3:00 PM")</span></span>
| <span data-ttu-id="190d0-130">**standard**</span><span class="sxs-lookup"><span data-stu-id="190d0-130">**standard**</span></span> | <span data-ttu-id="190d0-131">使用标准绝对表示形式（如</span><span class="sxs-lookup"><span data-stu-id="190d0-131">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="190d0-132">“2017 年 5 月 10 日下午 3:20”）</span><span class="sxs-lookup"><span data-stu-id="190d0-132">"5/10/2017 3:20 PM")</span></span>


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

