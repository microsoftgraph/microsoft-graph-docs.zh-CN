---
title: workbookApplication 资源类型
description: 表示管理工作簿的 Excel workbookApplication。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 3db8c640ebb2fd36a0902563c28a3ec51bfa99d8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348592"
---
# <a name="workbookapplication-resource-type"></a><span data-ttu-id="43dd2-103">workbookApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="43dd2-103">workbookApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43dd2-104">表示用于管理工作簿的 Excel 应用程序。</span><span class="sxs-lookup"><span data-stu-id="43dd2-104">Represents the Excel application that manages the workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="43dd2-105">方法</span><span class="sxs-lookup"><span data-stu-id="43dd2-105">Methods</span></span>

| <span data-ttu-id="43dd2-106">方法</span><span class="sxs-lookup"><span data-stu-id="43dd2-106">Method</span></span>           | <span data-ttu-id="43dd2-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="43dd2-107">Return Type</span></span>    |<span data-ttu-id="43dd2-108">说明</span><span class="sxs-lookup"><span data-stu-id="43dd2-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="43dd2-109">获取 workbookApplication</span><span class="sxs-lookup"><span data-stu-id="43dd2-109">Get workbookApplication</span></span>](../api/workbookapplication-get.md) | [<span data-ttu-id="43dd2-110">workbookApplication</span><span class="sxs-lookup"><span data-stu-id="43dd2-110">workbookApplication</span></span>](workbookapplication.md) |<span data-ttu-id="43dd2-111">读取 workbookApplication 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="43dd2-111">Read properties and relationships of workbookApplication object.</span></span>|
|[<span data-ttu-id="43dd2-112">Calculate</span><span class="sxs-lookup"><span data-stu-id="43dd2-112">Calculate</span></span>](../api/workbookapplication-calculate.md)|<span data-ttu-id="43dd2-113">无</span><span class="sxs-lookup"><span data-stu-id="43dd2-113">None</span></span>|<span data-ttu-id="43dd2-114">重新计算 Excel 中当前打开的所有工作簿。</span><span class="sxs-lookup"><span data-stu-id="43dd2-114">Recalculate all currently opened workbooks in Excel.</span></span>|

## <a name="properties"></a><span data-ttu-id="43dd2-115">属性</span><span class="sxs-lookup"><span data-stu-id="43dd2-115">Properties</span></span>
| <span data-ttu-id="43dd2-116">属性</span><span class="sxs-lookup"><span data-stu-id="43dd2-116">Property</span></span>     | <span data-ttu-id="43dd2-117">类型</span><span class="sxs-lookup"><span data-stu-id="43dd2-117">Type</span></span>   |<span data-ttu-id="43dd2-118">说明</span><span class="sxs-lookup"><span data-stu-id="43dd2-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="43dd2-119">calculationMode</span><span class="sxs-lookup"><span data-stu-id="43dd2-119">calculationMode</span></span>|<span data-ttu-id="43dd2-120">string</span><span class="sxs-lookup"><span data-stu-id="43dd2-120">string</span></span>|<span data-ttu-id="43dd2-121">返回工作簿中使用的计算模式。</span><span class="sxs-lookup"><span data-stu-id="43dd2-121">Returns the calculation mode used in the workbook.</span></span> <span data-ttu-id="43dd2-122">可取值为：`Automatic`、`AutomaticExceptTables`、`Manual`。</span><span class="sxs-lookup"><span data-stu-id="43dd2-122">Possible values are: `Automatic`, `AutomaticExceptTables`, `Manual`.</span></span> <span data-ttu-id="43dd2-123">只读。</span><span class="sxs-lookup"><span data-stu-id="43dd2-123">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="43dd2-124">关系</span><span class="sxs-lookup"><span data-stu-id="43dd2-124">Relationships</span></span>
<span data-ttu-id="43dd2-125">无</span><span class="sxs-lookup"><span data-stu-id="43dd2-125">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="43dd2-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="43dd2-126">JSON representation</span></span>

<span data-ttu-id="43dd2-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="43dd2-127">Here is a JSON representation of the resource.</span></span>

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
