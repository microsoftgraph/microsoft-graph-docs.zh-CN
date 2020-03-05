---
title: workbookApplication 资源类型
description: 表示用于管理工作簿的 Excel 应用程序。
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: d4b2833910d22696ee95ed707469f6da2068453c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446721"
---
# <a name="workbookapplication-resource-type"></a><span data-ttu-id="d2fc2-103">workbookApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="d2fc2-103">workbookApplication resource type</span></span>

<span data-ttu-id="d2fc2-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d2fc2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d2fc2-105">表示用于管理工作簿的 Excel 应用程序。</span><span class="sxs-lookup"><span data-stu-id="d2fc2-105">Represents the Excel application that manages the workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="d2fc2-106">方法</span><span class="sxs-lookup"><span data-stu-id="d2fc2-106">Methods</span></span>

| <span data-ttu-id="d2fc2-107">方法</span><span class="sxs-lookup"><span data-stu-id="d2fc2-107">Method</span></span>           | <span data-ttu-id="d2fc2-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="d2fc2-108">Return Type</span></span>    |<span data-ttu-id="d2fc2-109">说明</span><span class="sxs-lookup"><span data-stu-id="d2fc2-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d2fc2-110">获取 workbookApplication</span><span class="sxs-lookup"><span data-stu-id="d2fc2-110">Get workbookApplication</span></span>](../api/workbookapplication-get.md) | [<span data-ttu-id="d2fc2-111">workbookApplication</span><span class="sxs-lookup"><span data-stu-id="d2fc2-111">workbookApplication</span></span>](workbookapplication.md) |<span data-ttu-id="d2fc2-112">读取 workbookApplication 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d2fc2-112">Read properties and relationships of workbookApplication object.</span></span>|
|[<span data-ttu-id="d2fc2-113">Calculate</span><span class="sxs-lookup"><span data-stu-id="d2fc2-113">Calculate</span></span>](../api/workbookapplication-calculate.md)|<span data-ttu-id="d2fc2-114">无</span><span class="sxs-lookup"><span data-stu-id="d2fc2-114">None</span></span>|<span data-ttu-id="d2fc2-115">重新计算 Excel 中当前打开的所有工作簿。</span><span class="sxs-lookup"><span data-stu-id="d2fc2-115">Recalculate all currently opened workbooks in Excel.</span></span>|

## <a name="properties"></a><span data-ttu-id="d2fc2-116">属性</span><span class="sxs-lookup"><span data-stu-id="d2fc2-116">Properties</span></span>
| <span data-ttu-id="d2fc2-117">属性</span><span class="sxs-lookup"><span data-stu-id="d2fc2-117">Property</span></span>     | <span data-ttu-id="d2fc2-118">类型</span><span class="sxs-lookup"><span data-stu-id="d2fc2-118">Type</span></span>   |<span data-ttu-id="d2fc2-119">说明</span><span class="sxs-lookup"><span data-stu-id="d2fc2-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2fc2-120">calculationMode</span><span class="sxs-lookup"><span data-stu-id="d2fc2-120">calculationMode</span></span>|<span data-ttu-id="d2fc2-121">string</span><span class="sxs-lookup"><span data-stu-id="d2fc2-121">string</span></span>|<span data-ttu-id="d2fc2-122">返回工作簿中使用的计算模式。</span><span class="sxs-lookup"><span data-stu-id="d2fc2-122">Returns the calculation mode used in the workbook.</span></span> <span data-ttu-id="d2fc2-123">可取值为：`Automatic`、`AutomaticExceptTables`、`Manual`。</span><span class="sxs-lookup"><span data-stu-id="d2fc2-123">Possible values are: `Automatic`, `AutomaticExceptTables`, `Manual`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2fc2-124">关系</span><span class="sxs-lookup"><span data-stu-id="d2fc2-124">Relationships</span></span>
<span data-ttu-id="d2fc2-125">无。</span><span class="sxs-lookup"><span data-stu-id="d2fc2-125">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="d2fc2-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d2fc2-126">JSON representation</span></span>

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
