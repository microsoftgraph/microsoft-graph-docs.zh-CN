---
title: workbookApplication 资源类型
description: 表示用于管理工作簿的 Excel 应用程序。
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: a4f7d2cd6887598ac0a60522dc5bee1101dff9c9
ms.sourcegitcommit: 2f3e7325b5bc1f0cdc12a8acdf34d31cea3b8bdb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/07/2019
ms.locfileid: "38023246"
---
# <a name="workbookapplication-resource-type"></a><span data-ttu-id="a5d2b-103">workbookApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="a5d2b-103">workbookApplication resource type</span></span>

<span data-ttu-id="a5d2b-104">表示用于管理工作簿的 Excel 应用程序。</span><span class="sxs-lookup"><span data-stu-id="a5d2b-104">Represents the Excel application that manages the workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="a5d2b-105">方法</span><span class="sxs-lookup"><span data-stu-id="a5d2b-105">Methods</span></span>

| <span data-ttu-id="a5d2b-106">方法</span><span class="sxs-lookup"><span data-stu-id="a5d2b-106">Method</span></span>           | <span data-ttu-id="a5d2b-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="a5d2b-107">Return Type</span></span>    |<span data-ttu-id="a5d2b-108">说明</span><span class="sxs-lookup"><span data-stu-id="a5d2b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a5d2b-109">获取 workbookApplication</span><span class="sxs-lookup"><span data-stu-id="a5d2b-109">Get workbookApplication</span></span>](../api/workbookapplication-get.md) | [<span data-ttu-id="a5d2b-110">workbookApplication</span><span class="sxs-lookup"><span data-stu-id="a5d2b-110">workbookApplication</span></span>](workbookapplication.md) |<span data-ttu-id="a5d2b-111">读取 workbookApplication 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a5d2b-111">Read properties and relationships of workbookApplication object.</span></span>|
|[<span data-ttu-id="a5d2b-112">Calculate</span><span class="sxs-lookup"><span data-stu-id="a5d2b-112">Calculate</span></span>](../api/workbookapplication-calculate.md)|<span data-ttu-id="a5d2b-113">无</span><span class="sxs-lookup"><span data-stu-id="a5d2b-113">None</span></span>|<span data-ttu-id="a5d2b-114">重新计算 Excel 中当前打开的所有工作簿。</span><span class="sxs-lookup"><span data-stu-id="a5d2b-114">Recalculate all currently opened workbooks in Excel.</span></span>|

## <a name="properties"></a><span data-ttu-id="a5d2b-115">属性</span><span class="sxs-lookup"><span data-stu-id="a5d2b-115">Properties</span></span>
| <span data-ttu-id="a5d2b-116">属性</span><span class="sxs-lookup"><span data-stu-id="a5d2b-116">Property</span></span>     | <span data-ttu-id="a5d2b-117">类型</span><span class="sxs-lookup"><span data-stu-id="a5d2b-117">Type</span></span>   |<span data-ttu-id="a5d2b-118">说明</span><span class="sxs-lookup"><span data-stu-id="a5d2b-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5d2b-119">calculationMode</span><span class="sxs-lookup"><span data-stu-id="a5d2b-119">calculationMode</span></span>|<span data-ttu-id="a5d2b-120">string</span><span class="sxs-lookup"><span data-stu-id="a5d2b-120">string</span></span>|<span data-ttu-id="a5d2b-121">返回工作簿中使用的计算模式。</span><span class="sxs-lookup"><span data-stu-id="a5d2b-121">Returns the calculation mode used in the workbook.</span></span> <span data-ttu-id="a5d2b-122">可取值为：`Automatic`、`AutomaticExceptTables`、`Manual`。</span><span class="sxs-lookup"><span data-stu-id="a5d2b-122">Possible values are: `Automatic`, `AutomaticExceptTables`, `Manual`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5d2b-123">关系</span><span class="sxs-lookup"><span data-stu-id="a5d2b-123">Relationships</span></span>
<span data-ttu-id="a5d2b-124">无。</span><span class="sxs-lookup"><span data-stu-id="a5d2b-124">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="a5d2b-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a5d2b-125">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookApplication"
}-->

```json
{
  "calculationMode": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
