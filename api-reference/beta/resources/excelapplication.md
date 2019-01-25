---
title: 应用程序资源类型
description: 表示用于管理工作簿的 Excel 应用程序。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 48ee13a67d97f9c5c1a96a6ef6e104c5629f4108
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517615"
---
# <a name="application-resource-type"></a><span data-ttu-id="a2358-103">应用程序资源类型</span><span class="sxs-lookup"><span data-stu-id="a2358-103">Application resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2358-104">表示用于管理工作簿的 Excel 应用程序。</span><span class="sxs-lookup"><span data-stu-id="a2358-104">Represents the Excel application that manages the workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="a2358-105">方法</span><span class="sxs-lookup"><span data-stu-id="a2358-105">Methods</span></span>

| <span data-ttu-id="a2358-106">方法</span><span class="sxs-lookup"><span data-stu-id="a2358-106">Method</span></span>           | <span data-ttu-id="a2358-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="a2358-107">Return Type</span></span>    |<span data-ttu-id="a2358-108">说明</span><span class="sxs-lookup"><span data-stu-id="a2358-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2358-109">获取应用程序</span><span class="sxs-lookup"><span data-stu-id="a2358-109">[Get Application](../api/excelapplication-get.md)</span></span> | [<span data-ttu-id="a2358-110">Application</span><span class="sxs-lookup"><span data-stu-id="a2358-110">Application</span></span>](application.md) |<span data-ttu-id="a2358-111">读取属性和 application 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="a2358-111">Read properties and relationships of application object.</span></span>|
|[<span data-ttu-id="a2358-112">Calculate</span><span class="sxs-lookup"><span data-stu-id="a2358-112">Calculate</span></span>](../api/excelapplication-calculate.md)|<span data-ttu-id="a2358-113">无</span><span class="sxs-lookup"><span data-stu-id="a2358-113">None</span></span>|<span data-ttu-id="a2358-114">重新计算 Excel 中当前打开的所有工作簿。</span><span class="sxs-lookup"><span data-stu-id="a2358-114">Recalculate all currently opened workbooks in Excel.</span></span>|

## <a name="properties"></a><span data-ttu-id="a2358-115">属性</span><span class="sxs-lookup"><span data-stu-id="a2358-115">Properties</span></span>
| <span data-ttu-id="a2358-116">属性</span><span class="sxs-lookup"><span data-stu-id="a2358-116">Property</span></span>     | <span data-ttu-id="a2358-117">类型</span><span class="sxs-lookup"><span data-stu-id="a2358-117">Type</span></span>   |<span data-ttu-id="a2358-118">说明</span><span class="sxs-lookup"><span data-stu-id="a2358-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2358-119">calculationMode</span><span class="sxs-lookup"><span data-stu-id="a2358-119">calculationMode</span></span>|<span data-ttu-id="a2358-120">string</span><span class="sxs-lookup"><span data-stu-id="a2358-120">string</span></span>|<span data-ttu-id="a2358-121">返回工作簿中使用的计算模式。</span><span class="sxs-lookup"><span data-stu-id="a2358-121">Returns the calculation mode used in the workbook.</span></span> <span data-ttu-id="a2358-122">可取值为：`Automatic`、`AutomaticExceptTables`、`Manual`。</span><span class="sxs-lookup"><span data-stu-id="a2358-122">Possible values are: `Automatic`, `AutomaticExceptTables`, `Manual`.</span></span> <span data-ttu-id="a2358-123">只读。</span><span class="sxs-lookup"><span data-stu-id="a2358-123">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2358-124">关系</span><span class="sxs-lookup"><span data-stu-id="a2358-124">Relationships</span></span>
<span data-ttu-id="a2358-125">无</span><span class="sxs-lookup"><span data-stu-id="a2358-125">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a2358-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a2358-126">JSON representation</span></span>

<span data-ttu-id="a2358-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2358-127">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.application"
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
  "description": "Application resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/excelapplication.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
