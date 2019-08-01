---
title: FormatProtection 资源类型
description: 表示对范围对象的格式保护。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: babd1192e216179c59b40d78175f24b0e8366d71
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032436"
---
# <a name="formatprotection-resource-type"></a><span data-ttu-id="a9620-103">FormatProtection 资源类型</span><span class="sxs-lookup"><span data-stu-id="a9620-103">FormatProtection resource type</span></span>

<span data-ttu-id="a9620-104">表示对范围对象的格式保护。</span><span class="sxs-lookup"><span data-stu-id="a9620-104">Represents the format protection of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="a9620-105">方法</span><span class="sxs-lookup"><span data-stu-id="a9620-105">Methods</span></span>

| <span data-ttu-id="a9620-106">方法</span><span class="sxs-lookup"><span data-stu-id="a9620-106">Method</span></span>           | <span data-ttu-id="a9620-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="a9620-107">Return Type</span></span>    |<span data-ttu-id="a9620-108">说明</span><span class="sxs-lookup"><span data-stu-id="a9620-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a9620-109">获取 FormatProtection</span><span class="sxs-lookup"><span data-stu-id="a9620-109">Get FormatProtection</span></span>](../api/formatprotection-get.md) | [<span data-ttu-id="a9620-110">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="a9620-110">FormatProtection</span></span>](formatprotection.md) |<span data-ttu-id="a9620-111">读取 formatProtection 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a9620-111">Read properties and relationships of formatProtection object.</span></span>|
|[<span data-ttu-id="a9620-112">更新</span><span class="sxs-lookup"><span data-stu-id="a9620-112">Update</span></span>](../api/formatprotection-update.md) | [<span data-ttu-id="a9620-113">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="a9620-113">FormatProtection</span></span>](formatprotection.md)  |<span data-ttu-id="a9620-114">更新 FormatProtection 对象。</span><span class="sxs-lookup"><span data-stu-id="a9620-114">Update FormatProtection object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a9620-115">属性</span><span class="sxs-lookup"><span data-stu-id="a9620-115">Properties</span></span>
| <span data-ttu-id="a9620-116">属性</span><span class="sxs-lookup"><span data-stu-id="a9620-116">Property</span></span>     | <span data-ttu-id="a9620-117">类型</span><span class="sxs-lookup"><span data-stu-id="a9620-117">Type</span></span>   |<span data-ttu-id="a9620-118">说明</span><span class="sxs-lookup"><span data-stu-id="a9620-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9620-119">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="a9620-119">formulaHidden</span></span>|<span data-ttu-id="a9620-120">boolean</span><span class="sxs-lookup"><span data-stu-id="a9620-120">boolean</span></span>|<span data-ttu-id="a9620-p101">表示 Excel 是否隐藏区域中的单元格公式。指示整个区域不具有统一公式隐藏设置的空值。</span><span class="sxs-lookup"><span data-stu-id="a9620-p101">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="a9620-123">已锁定</span><span class="sxs-lookup"><span data-stu-id="a9620-123">locked</span></span>|<span data-ttu-id="a9620-124">boolean</span><span class="sxs-lookup"><span data-stu-id="a9620-124">boolean</span></span>|<span data-ttu-id="a9620-p102">指示 Excel 是否锁定对象中的单元格。指示整个区域不具有统一锁定设置的空值。</span><span class="sxs-lookup"><span data-stu-id="a9620-p102">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9620-127">关系</span><span class="sxs-lookup"><span data-stu-id="a9620-127">Relationships</span></span>
<span data-ttu-id="a9620-128">无</span><span class="sxs-lookup"><span data-stu-id="a9620-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a9620-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a9620-129">JSON representation</span></span>

<span data-ttu-id="a9620-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a9620-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFormatProtection"
}-->

```json
{
  "formulaHidden": true,
  "locked": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "FormatProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
