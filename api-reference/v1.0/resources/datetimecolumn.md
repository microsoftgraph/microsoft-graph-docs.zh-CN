---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: DateTimeColumn
localization_priority: Normal
ms.openlocfilehash: ba650ccbe307ba286cf2182bda35a21f3c675114
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574762"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="67b24-102">DateTimeColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="67b24-102">DateTimeColumn resource type</span></span>

<span data-ttu-id="67b24-103">[columnDefinition](columndefinition.md) 资源上的 **dateTimeColumn** 指示该列的值为日期或时间。</span><span class="sxs-lookup"><span data-stu-id="67b24-103">The **dateTimeColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="67b24-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="67b24-104">JSON representation</span></span>

<span data-ttu-id="67b24-105">下面是 **dateTimeColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="67b24-105">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="67b24-106">属性</span><span class="sxs-lookup"><span data-stu-id="67b24-106">Properties</span></span>

| <span data-ttu-id="67b24-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="67b24-107">Property name</span></span>      | <span data-ttu-id="67b24-108">类型</span><span class="sxs-lookup"><span data-stu-id="67b24-108">Type</span></span>               | <span data-ttu-id="67b24-109">说明</span><span class="sxs-lookup"><span data-stu-id="67b24-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="67b24-110">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="67b24-110">**displayAs**</span></span>      | <span data-ttu-id="67b24-111">string</span><span class="sxs-lookup"><span data-stu-id="67b24-111">string</span></span>             | <span data-ttu-id="67b24-112">值在用户体验中的显示方式。</span><span class="sxs-lookup"><span data-stu-id="67b24-112">How the value should be presented in the UX.</span></span> <span data-ttu-id="67b24-113">必须为 `default`、`friendly` 或 `standard` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="67b24-113">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="67b24-114">有关详细信息，请参阅下文。</span><span class="sxs-lookup"><span data-stu-id="67b24-114">See below for more details.</span></span> <span data-ttu-id="67b24-115">如果未指定，则视为 `default`。</span><span class="sxs-lookup"><span data-stu-id="67b24-115">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="67b24-116">**format**</span><span class="sxs-lookup"><span data-stu-id="67b24-116">**format**</span></span>         | <span data-ttu-id="67b24-117">string</span><span class="sxs-lookup"><span data-stu-id="67b24-117">string</span></span>             | <span data-ttu-id="67b24-118">指示值是否应该只显示为日期或日期和时间。</span><span class="sxs-lookup"><span data-stu-id="67b24-118">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="67b24-119">必须为 `dateOnly` 或 `dateTime` 的其中一个</span><span class="sxs-lookup"><span data-stu-id="67b24-119">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-options"></a><span data-ttu-id="67b24-120">DisplayAs 选项</span><span class="sxs-lookup"><span data-stu-id="67b24-120">DisplayAs options</span></span>

| <span data-ttu-id="67b24-121">值</span><span class="sxs-lookup"><span data-stu-id="67b24-121">Value</span></span>        | <span data-ttu-id="67b24-122">说明</span><span class="sxs-lookup"><span data-stu-id="67b24-122">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="67b24-123">**default**</span><span class="sxs-lookup"><span data-stu-id="67b24-123">**default**</span></span>  | <span data-ttu-id="67b24-124">使用用户体验中呈现的默认值。</span><span class="sxs-lookup"><span data-stu-id="67b24-124">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="67b24-125">**friendly**</span><span class="sxs-lookup"><span data-stu-id="67b24-125">**friendly**</span></span> | <span data-ttu-id="67b24-126">使用友好相对表示形式（如</span><span class="sxs-lookup"><span data-stu-id="67b24-126">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="67b24-127">“今天下午 3:00”）</span><span class="sxs-lookup"><span data-stu-id="67b24-127">"today at 3:00 PM")</span></span>
| <span data-ttu-id="67b24-128">**standard**</span><span class="sxs-lookup"><span data-stu-id="67b24-128">**standard**</span></span> | <span data-ttu-id="67b24-129">使用标准绝对表示形式（如</span><span class="sxs-lookup"><span data-stu-id="67b24-129">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="67b24-130">“2017 年 5 月 10 日下午 3:20”）</span><span class="sxs-lookup"><span data-stu-id="67b24-130">"5/10/2017 3:20 PM")</span></span>


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
