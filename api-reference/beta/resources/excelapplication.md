---
title: 应用程序资源类型
description: 表示用于管理工作簿的 Excel 应用程序。
ms.openlocfilehash: 1772d69b55d03bf62d983a6dfb818dca651ebbd6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044703"
---
# <a name="application-resource-type"></a><span data-ttu-id="8500e-103">应用程序资源类型</span><span class="sxs-lookup"><span data-stu-id="8500e-103">Application resource type</span></span>

> <span data-ttu-id="8500e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8500e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8500e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8500e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8500e-106">表示用于管理工作簿的 Excel 应用程序。</span><span class="sxs-lookup"><span data-stu-id="8500e-106">Represents the Excel application that manages the workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="8500e-107">方法</span><span class="sxs-lookup"><span data-stu-id="8500e-107">Methods</span></span>

| <span data-ttu-id="8500e-108">方法</span><span class="sxs-lookup"><span data-stu-id="8500e-108">Method</span></span>           | <span data-ttu-id="8500e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="8500e-109">Return Type</span></span>    |<span data-ttu-id="8500e-110">说明</span><span class="sxs-lookup"><span data-stu-id="8500e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8500e-111">获取应用程序</span><span class="sxs-lookup"><span data-stu-id="8500e-111">Get Application</span></span>](../api/excelapplication-get.md) | [<span data-ttu-id="8500e-112">Application</span><span class="sxs-lookup"><span data-stu-id="8500e-112">Application</span></span>](application.md) |<span data-ttu-id="8500e-113">读取属性和 application 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="8500e-113">Read properties and relationships of application object.</span></span>|
|[<span data-ttu-id="8500e-114">Calculate</span><span class="sxs-lookup"><span data-stu-id="8500e-114">Calculate</span></span>](../api/excelapplication-calculate.md)|<span data-ttu-id="8500e-115">无</span><span class="sxs-lookup"><span data-stu-id="8500e-115">None</span></span>|<span data-ttu-id="8500e-116">重新计算 Excel 中当前打开的所有工作簿。</span><span class="sxs-lookup"><span data-stu-id="8500e-116">Recalculate all currently opened workbooks in Excel.</span></span>|

## <a name="properties"></a><span data-ttu-id="8500e-117">属性</span><span class="sxs-lookup"><span data-stu-id="8500e-117">Properties</span></span>
| <span data-ttu-id="8500e-118">属性</span><span class="sxs-lookup"><span data-stu-id="8500e-118">Property</span></span>     | <span data-ttu-id="8500e-119">类型</span><span class="sxs-lookup"><span data-stu-id="8500e-119">Type</span></span>   |<span data-ttu-id="8500e-120">说明</span><span class="sxs-lookup"><span data-stu-id="8500e-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8500e-121">calculationMode</span><span class="sxs-lookup"><span data-stu-id="8500e-121">calculationMode</span></span>|<span data-ttu-id="8500e-122">string</span><span class="sxs-lookup"><span data-stu-id="8500e-122">string</span></span>|<span data-ttu-id="8500e-123">返回工作簿中使用的计算模式。</span><span class="sxs-lookup"><span data-stu-id="8500e-123">Returns the calculation mode used in the workbook.</span></span> <span data-ttu-id="8500e-124">可取值为：`Automatic`、`AutomaticExceptTables`、`Manual`。</span><span class="sxs-lookup"><span data-stu-id="8500e-124">Possible values are: `Automatic`, `AutomaticExceptTables`, `Manual`.</span></span> <span data-ttu-id="8500e-125">只读。</span><span class="sxs-lookup"><span data-stu-id="8500e-125">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8500e-126">Relationships</span><span class="sxs-lookup"><span data-stu-id="8500e-126">Relationships</span></span>
<span data-ttu-id="8500e-127">无</span><span class="sxs-lookup"><span data-stu-id="8500e-127">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8500e-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8500e-128">JSON representation</span></span>

<span data-ttu-id="8500e-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8500e-129">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Application resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->