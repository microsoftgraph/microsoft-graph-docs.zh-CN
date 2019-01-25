---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: DateTimeColumn
localization_priority: Normal
ms.openlocfilehash: e49b749adeaf7b04f9324fe00f9c73bf61f8b2dc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518679"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="f02fe-102">DateTimeColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="f02fe-102">DateTimeColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f02fe-103">[columnDefinition](columndefinition.md) 资源上的 **dateTimeColumn** 指示该列的值为日期或时间。</span><span class="sxs-lookup"><span data-stu-id="f02fe-103">The **dateTimeColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f02fe-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f02fe-104">JSON representation</span></span>

<span data-ttu-id="f02fe-105">下面是 **dateTimeColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f02fe-105">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="f02fe-106">属性</span><span class="sxs-lookup"><span data-stu-id="f02fe-106">Properties</span></span>

| <span data-ttu-id="f02fe-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="f02fe-107">Property name</span></span>      | <span data-ttu-id="f02fe-108">类型</span><span class="sxs-lookup"><span data-stu-id="f02fe-108">Type</span></span>               | <span data-ttu-id="f02fe-109">说明</span><span class="sxs-lookup"><span data-stu-id="f02fe-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="f02fe-110">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="f02fe-110">**displayAs**</span></span>      | <span data-ttu-id="f02fe-111">string</span><span class="sxs-lookup"><span data-stu-id="f02fe-111">string</span></span>             | <span data-ttu-id="f02fe-112">值在用户体验中的显示方式。</span><span class="sxs-lookup"><span data-stu-id="f02fe-112">How the value should be presented in the UX.</span></span> <span data-ttu-id="f02fe-113">必须为 `default`、`friendly` 或 `standard` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="f02fe-113">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="f02fe-114">有关详细信息，请参阅下文。</span><span class="sxs-lookup"><span data-stu-id="f02fe-114">See below for more details.</span></span> <span data-ttu-id="f02fe-115">如果未指定，则视为 `default`。</span><span class="sxs-lookup"><span data-stu-id="f02fe-115">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="f02fe-116">**format**</span><span class="sxs-lookup"><span data-stu-id="f02fe-116">**format**</span></span>         | <span data-ttu-id="f02fe-117">string</span><span class="sxs-lookup"><span data-stu-id="f02fe-117">string</span></span>             | <span data-ttu-id="f02fe-118">指示值是否应该只显示为日期或日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f02fe-118">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="f02fe-119">必须为 `dateOnly` 或 `dateTime` 的其中一个</span><span class="sxs-lookup"><span data-stu-id="f02fe-119">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-values"></a><span data-ttu-id="f02fe-120">DisplayAs 值</span><span class="sxs-lookup"><span data-stu-id="f02fe-120">DisplayAs values</span></span>

| <span data-ttu-id="f02fe-121">值</span><span class="sxs-lookup"><span data-stu-id="f02fe-121">Value</span></span>        | <span data-ttu-id="f02fe-122">说明</span><span class="sxs-lookup"><span data-stu-id="f02fe-122">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="f02fe-123">**default**</span><span class="sxs-lookup"><span data-stu-id="f02fe-123">**default**</span></span>  | <span data-ttu-id="f02fe-124">使用用户体验中呈现的默认值。</span><span class="sxs-lookup"><span data-stu-id="f02fe-124">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="f02fe-125">**friendly**</span><span class="sxs-lookup"><span data-stu-id="f02fe-125">**friendly**</span></span> | <span data-ttu-id="f02fe-126">使用友好相对表示形式（如</span><span class="sxs-lookup"><span data-stu-id="f02fe-126">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="f02fe-127">“今天下午 3:00”）</span><span class="sxs-lookup"><span data-stu-id="f02fe-127">"today at 3:00 PM")</span></span>
| <span data-ttu-id="f02fe-128">**standard**</span><span class="sxs-lookup"><span data-stu-id="f02fe-128">**standard**</span></span> | <span data-ttu-id="f02fe-129">使用标准绝对表示形式（如</span><span class="sxs-lookup"><span data-stu-id="f02fe-129">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="f02fe-130">“2017 年 5 月 10 日下午 3:20”）</span><span class="sxs-lookup"><span data-stu-id="f02fe-130">"5/10/2017 3:20 PM")</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DateTimeColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/datetimecolumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
