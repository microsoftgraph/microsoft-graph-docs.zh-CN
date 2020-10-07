---
title: workbookApplication 资源类型
description: 表示管理工作簿的 Excel workbookApplication。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 4616b3e61fbea3b918ef897ebe69dd12ffb0dbb2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039172"
---
# <a name="workbookapplication-resource-type"></a><span data-ttu-id="711cc-103">workbookApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="711cc-103">workbookApplication resource type</span></span>

<span data-ttu-id="711cc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="711cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="711cc-105">表示用于管理工作簿的 Excel 应用程序。</span><span class="sxs-lookup"><span data-stu-id="711cc-105">Represents the Excel application that manages the workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="711cc-106">方法</span><span class="sxs-lookup"><span data-stu-id="711cc-106">Methods</span></span>

| <span data-ttu-id="711cc-107">方法</span><span class="sxs-lookup"><span data-stu-id="711cc-107">Method</span></span>           | <span data-ttu-id="711cc-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="711cc-108">Return Type</span></span>    |<span data-ttu-id="711cc-109">说明</span><span class="sxs-lookup"><span data-stu-id="711cc-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="711cc-110">获取 workbookApplication</span><span class="sxs-lookup"><span data-stu-id="711cc-110">Get workbookApplication</span></span>](../api/workbookapplication-get.md) | [<span data-ttu-id="711cc-111">workbookApplication</span><span class="sxs-lookup"><span data-stu-id="711cc-111">workbookApplication</span></span>](workbookapplication.md) |<span data-ttu-id="711cc-112">读取 workbookApplication 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="711cc-112">Read properties and relationships of workbookApplication object.</span></span>|
|[<span data-ttu-id="711cc-113">Calculate</span><span class="sxs-lookup"><span data-stu-id="711cc-113">Calculate</span></span>](../api/workbookapplication-calculate.md)|<span data-ttu-id="711cc-114">无</span><span class="sxs-lookup"><span data-stu-id="711cc-114">None</span></span>|<span data-ttu-id="711cc-115">重新计算 Excel 中当前打开的所有工作簿。</span><span class="sxs-lookup"><span data-stu-id="711cc-115">Recalculate all currently opened workbooks in Excel.</span></span>|

## <a name="properties"></a><span data-ttu-id="711cc-116">属性</span><span class="sxs-lookup"><span data-stu-id="711cc-116">Properties</span></span>
| <span data-ttu-id="711cc-117">属性</span><span class="sxs-lookup"><span data-stu-id="711cc-117">Property</span></span>     | <span data-ttu-id="711cc-118">类型</span><span class="sxs-lookup"><span data-stu-id="711cc-118">Type</span></span>   |<span data-ttu-id="711cc-119">说明</span><span class="sxs-lookup"><span data-stu-id="711cc-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="711cc-120">calculationMode</span><span class="sxs-lookup"><span data-stu-id="711cc-120">calculationMode</span></span>|<span data-ttu-id="711cc-121">string</span><span class="sxs-lookup"><span data-stu-id="711cc-121">string</span></span>|<span data-ttu-id="711cc-122">返回工作簿中使用的计算模式。</span><span class="sxs-lookup"><span data-stu-id="711cc-122">Returns the calculation mode used in the workbook.</span></span> <span data-ttu-id="711cc-123">可取值为：`Automatic`、`AutomaticExceptTables`、`Manual`。</span><span class="sxs-lookup"><span data-stu-id="711cc-123">Possible values are: `Automatic`, `AutomaticExceptTables`, `Manual`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="711cc-124">关系</span><span class="sxs-lookup"><span data-stu-id="711cc-124">Relationships</span></span>
<span data-ttu-id="711cc-125">无。</span><span class="sxs-lookup"><span data-stu-id="711cc-125">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="711cc-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="711cc-126">JSON representation</span></span>


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


