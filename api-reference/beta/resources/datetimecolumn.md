---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: DateTimeColumn
localization_priority: Normal
ms.openlocfilehash: 03ebb78adda52a9f98aec6635bbda48dd61e37e2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889213"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="d57df-102">DateTimeColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="d57df-102">DateTimeColumn resource type</span></span>

> <span data-ttu-id="d57df-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d57df-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d57df-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d57df-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d57df-105">[columnDefinition](columndefinition.md) 资源上的 **dateTimeColumn** 指示该列的值为日期或时间。</span><span class="sxs-lookup"><span data-stu-id="d57df-105">The **dateTimeColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d57df-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d57df-106">JSON representation</span></span>

<span data-ttu-id="d57df-107">下面是 **dateTimeColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d57df-107">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="d57df-108">属性</span><span class="sxs-lookup"><span data-stu-id="d57df-108">Properties</span></span>

| <span data-ttu-id="d57df-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="d57df-109">Property name</span></span>      | <span data-ttu-id="d57df-110">类型</span><span class="sxs-lookup"><span data-stu-id="d57df-110">Type</span></span>               | <span data-ttu-id="d57df-111">说明</span><span class="sxs-lookup"><span data-stu-id="d57df-111">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="d57df-112">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="d57df-112">**displayAs**</span></span>      | <span data-ttu-id="d57df-113">string</span><span class="sxs-lookup"><span data-stu-id="d57df-113">string</span></span>             | <span data-ttu-id="d57df-114">值在用户体验中的显示方式。</span><span class="sxs-lookup"><span data-stu-id="d57df-114">How the value should be presented in the UX.</span></span> <span data-ttu-id="d57df-115">必须为 `default`、`friendly` 或 `standard` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="d57df-115">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="d57df-116">有关详细信息，请参阅下文。</span><span class="sxs-lookup"><span data-stu-id="d57df-116">See below for more details.</span></span> <span data-ttu-id="d57df-117">如果未指定，则视为 `default`。</span><span class="sxs-lookup"><span data-stu-id="d57df-117">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="d57df-118">**format**</span><span class="sxs-lookup"><span data-stu-id="d57df-118">**format**</span></span>         | <span data-ttu-id="d57df-119">string</span><span class="sxs-lookup"><span data-stu-id="d57df-119">string</span></span>             | <span data-ttu-id="d57df-120">指示值是否应该只显示为日期或日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d57df-120">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="d57df-121">必须为 `dateOnly` 或 `dateTime` 的其中一个</span><span class="sxs-lookup"><span data-stu-id="d57df-121">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-values"></a><span data-ttu-id="d57df-122">DisplayAs 值</span><span class="sxs-lookup"><span data-stu-id="d57df-122">DisplayAs values</span></span>

| <span data-ttu-id="d57df-123">值</span><span class="sxs-lookup"><span data-stu-id="d57df-123">Value</span></span>        | <span data-ttu-id="d57df-124">说明</span><span class="sxs-lookup"><span data-stu-id="d57df-124">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="d57df-125">**default**</span><span class="sxs-lookup"><span data-stu-id="d57df-125">**default**</span></span>  | <span data-ttu-id="d57df-126">使用用户体验中呈现的默认值。</span><span class="sxs-lookup"><span data-stu-id="d57df-126">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="d57df-127">**friendly**</span><span class="sxs-lookup"><span data-stu-id="d57df-127">**friendly**</span></span> | <span data-ttu-id="d57df-128">使用友好相对表示形式（如</span><span class="sxs-lookup"><span data-stu-id="d57df-128">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="d57df-129">“今天下午 3:00”）</span><span class="sxs-lookup"><span data-stu-id="d57df-129">"today at 3:00 PM")</span></span>
| <span data-ttu-id="d57df-130">**standard**</span><span class="sxs-lookup"><span data-stu-id="d57df-130">**standard**</span></span> | <span data-ttu-id="d57df-131">使用标准绝对表示形式（如</span><span class="sxs-lookup"><span data-stu-id="d57df-131">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="d57df-132">“2017 年 5 月 10 日下午 3:20”）</span><span class="sxs-lookup"><span data-stu-id="d57df-132">"5/10/2017 3:20 PM")</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DateTimeColumn"
} -->
