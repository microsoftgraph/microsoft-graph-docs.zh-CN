---
title: workbookApplication 资源类型
description: 表示管理工作簿的 Excel workbookApplication。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 71c7c92e623fc2a9c05b9e1e8448f329615c51e3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964107"
---
# <a name="workbookapplication-resource-type"></a><span data-ttu-id="6c9d6-103">workbookApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="6c9d6-103">workbookApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c9d6-104">表示用于管理工作簿的 Excel 应用程序。</span><span class="sxs-lookup"><span data-stu-id="6c9d6-104">Represents the Excel application that manages the workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="6c9d6-105">方法</span><span class="sxs-lookup"><span data-stu-id="6c9d6-105">Methods</span></span>

| <span data-ttu-id="6c9d6-106">方法</span><span class="sxs-lookup"><span data-stu-id="6c9d6-106">Method</span></span>           | <span data-ttu-id="6c9d6-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="6c9d6-107">Return Type</span></span>    |<span data-ttu-id="6c9d6-108">说明</span><span class="sxs-lookup"><span data-stu-id="6c9d6-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6c9d6-109">获取 workbookApplication</span><span class="sxs-lookup"><span data-stu-id="6c9d6-109">Get workbookApplication</span></span>](../api/workbookapplication-get.md) | [<span data-ttu-id="6c9d6-110">workbookApplication</span><span class="sxs-lookup"><span data-stu-id="6c9d6-110">workbookApplication</span></span>](workbookapplication.md) |<span data-ttu-id="6c9d6-111">读取 workbookApplication 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6c9d6-111">Read properties and relationships of workbookApplication object.</span></span>|
|[<span data-ttu-id="6c9d6-112">Calculate</span><span class="sxs-lookup"><span data-stu-id="6c9d6-112">Calculate</span></span>](../api/workbookapplication-calculate.md)|<span data-ttu-id="6c9d6-113">无</span><span class="sxs-lookup"><span data-stu-id="6c9d6-113">None</span></span>|<span data-ttu-id="6c9d6-114">重新计算 Excel 中当前打开的所有工作簿。</span><span class="sxs-lookup"><span data-stu-id="6c9d6-114">Recalculate all currently opened workbooks in Excel.</span></span>|

## <a name="properties"></a><span data-ttu-id="6c9d6-115">属性</span><span class="sxs-lookup"><span data-stu-id="6c9d6-115">Properties</span></span>
| <span data-ttu-id="6c9d6-116">属性</span><span class="sxs-lookup"><span data-stu-id="6c9d6-116">Property</span></span>     | <span data-ttu-id="6c9d6-117">类型</span><span class="sxs-lookup"><span data-stu-id="6c9d6-117">Type</span></span>   |<span data-ttu-id="6c9d6-118">说明</span><span class="sxs-lookup"><span data-stu-id="6c9d6-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c9d6-119">calculationMode</span><span class="sxs-lookup"><span data-stu-id="6c9d6-119">calculationMode</span></span>|<span data-ttu-id="6c9d6-120">string</span><span class="sxs-lookup"><span data-stu-id="6c9d6-120">string</span></span>|<span data-ttu-id="6c9d6-121">返回工作簿中使用的计算模式。</span><span class="sxs-lookup"><span data-stu-id="6c9d6-121">Returns the calculation mode used in the workbook.</span></span> <span data-ttu-id="6c9d6-122">可取值为：`Automatic`、`AutomaticExceptTables`、`Manual`。</span><span class="sxs-lookup"><span data-stu-id="6c9d6-122">Possible values are: `Automatic`, `AutomaticExceptTables`, `Manual`.</span></span> <span data-ttu-id="6c9d6-123">只读。</span><span class="sxs-lookup"><span data-stu-id="6c9d6-123">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c9d6-124">关系</span><span class="sxs-lookup"><span data-stu-id="6c9d6-124">Relationships</span></span>
<span data-ttu-id="6c9d6-125">无</span><span class="sxs-lookup"><span data-stu-id="6c9d6-125">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6c9d6-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c9d6-126">JSON representation</span></span>

<span data-ttu-id="6c9d6-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c9d6-127">Here is a JSON representation of the resource.</span></span>

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
