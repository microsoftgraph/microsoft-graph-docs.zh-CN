---
author: JeremyKelley
description: columnDefinition 资源上的 dateTimeColumn 指示该列的值为日期或时间。
ms.date: 09/11/2017
title: DateTimeColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: e0e69e4019530031966cde9f782c2f017ba976fb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973882"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="ce096-103">DateTimeColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="ce096-103">DateTimeColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce096-104">[columnDefinition](columndefinition.md) 资源上的 **dateTimeColumn** 指示该列的值为日期或时间。</span><span class="sxs-lookup"><span data-stu-id="ce096-104">The **dateTimeColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce096-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ce096-105">JSON representation</span></span>

<span data-ttu-id="ce096-106">下面是 **dateTimeColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ce096-106">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="ce096-107">属性</span><span class="sxs-lookup"><span data-stu-id="ce096-107">Properties</span></span>

| <span data-ttu-id="ce096-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="ce096-108">Property name</span></span>      | <span data-ttu-id="ce096-109">类型</span><span class="sxs-lookup"><span data-stu-id="ce096-109">Type</span></span>               | <span data-ttu-id="ce096-110">说明</span><span class="sxs-lookup"><span data-stu-id="ce096-110">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="ce096-111">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="ce096-111">**displayAs**</span></span>      | <span data-ttu-id="ce096-112">string</span><span class="sxs-lookup"><span data-stu-id="ce096-112">string</span></span>             | <span data-ttu-id="ce096-113">值在用户体验中的显示方式。</span><span class="sxs-lookup"><span data-stu-id="ce096-113">How the value should be presented in the UX.</span></span> <span data-ttu-id="ce096-114">必须为 `default`、`friendly` 或 `standard` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="ce096-114">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="ce096-115">有关详细信息，请参阅下文。</span><span class="sxs-lookup"><span data-stu-id="ce096-115">See below for more details.</span></span> <span data-ttu-id="ce096-116">如果未指定，则视为 `default`。</span><span class="sxs-lookup"><span data-stu-id="ce096-116">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="ce096-117">**format**</span><span class="sxs-lookup"><span data-stu-id="ce096-117">**format**</span></span>         | <span data-ttu-id="ce096-118">string</span><span class="sxs-lookup"><span data-stu-id="ce096-118">string</span></span>             | <span data-ttu-id="ce096-119">指示值是否应该只显示为日期或日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ce096-119">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="ce096-120">必须为 `dateOnly` 或 `dateTime` 的其中一个</span><span class="sxs-lookup"><span data-stu-id="ce096-120">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-values"></a><span data-ttu-id="ce096-121">DisplayAs 值</span><span class="sxs-lookup"><span data-stu-id="ce096-121">DisplayAs values</span></span>

| <span data-ttu-id="ce096-122">值</span><span class="sxs-lookup"><span data-stu-id="ce096-122">Value</span></span>        | <span data-ttu-id="ce096-123">说明</span><span class="sxs-lookup"><span data-stu-id="ce096-123">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="ce096-124">**default**</span><span class="sxs-lookup"><span data-stu-id="ce096-124">**default**</span></span>  | <span data-ttu-id="ce096-125">使用用户体验中呈现的默认值。</span><span class="sxs-lookup"><span data-stu-id="ce096-125">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="ce096-126">**friendly**</span><span class="sxs-lookup"><span data-stu-id="ce096-126">**friendly**</span></span> | <span data-ttu-id="ce096-127">使用友好相对表示形式（如</span><span class="sxs-lookup"><span data-stu-id="ce096-127">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="ce096-128">“今天下午 3:00”）</span><span class="sxs-lookup"><span data-stu-id="ce096-128">"today at 3:00 PM")</span></span>
| <span data-ttu-id="ce096-129">**standard**</span><span class="sxs-lookup"><span data-stu-id="ce096-129">**standard**</span></span> | <span data-ttu-id="ce096-130">使用标准绝对表示形式（如</span><span class="sxs-lookup"><span data-stu-id="ce096-130">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="ce096-131">“2017 年 5 月 10 日下午 3:20”）</span><span class="sxs-lookup"><span data-stu-id="ce096-131">"5/10/2017 3:20 PM")</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DateTimeColumn",
  "suppressions": []
}
-->
