---
title: FormatProtection 资源类型
description: 表示对范围对象的格式保护。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e474a29e657d19e06aa35fbebffeee85d855acfa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531377"
---
# <a name="formatprotection-resource-type"></a><span data-ttu-id="9b103-103">FormatProtection 资源类型</span><span class="sxs-lookup"><span data-stu-id="9b103-103">FormatProtection resource type</span></span>

<span data-ttu-id="9b103-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b103-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9b103-105">表示对范围对象的格式保护。</span><span class="sxs-lookup"><span data-stu-id="9b103-105">Represents the format protection of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="9b103-106">Methods</span><span class="sxs-lookup"><span data-stu-id="9b103-106">Methods</span></span>

| <span data-ttu-id="9b103-107">方法</span><span class="sxs-lookup"><span data-stu-id="9b103-107">Method</span></span>           | <span data-ttu-id="9b103-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="9b103-108">Return Type</span></span>    |<span data-ttu-id="9b103-109">说明</span><span class="sxs-lookup"><span data-stu-id="9b103-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9b103-110">获取 FormatProtection</span><span class="sxs-lookup"><span data-stu-id="9b103-110">Get FormatProtection</span></span>](../api/formatprotection-get.md) | [<span data-ttu-id="9b103-111">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="9b103-111">FormatProtection</span></span>](formatprotection.md) |<span data-ttu-id="9b103-112">读取 formatProtection 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9b103-112">Read properties and relationships of formatProtection object.</span></span>|
|[<span data-ttu-id="9b103-113">更新</span><span class="sxs-lookup"><span data-stu-id="9b103-113">Update</span></span>](../api/formatprotection-update.md) | [<span data-ttu-id="9b103-114">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="9b103-114">FormatProtection</span></span>](formatprotection.md)  |<span data-ttu-id="9b103-115">更新 FormatProtection 对象。</span><span class="sxs-lookup"><span data-stu-id="9b103-115">Update FormatProtection object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9b103-116">属性</span><span class="sxs-lookup"><span data-stu-id="9b103-116">Properties</span></span>
| <span data-ttu-id="9b103-117">属性</span><span class="sxs-lookup"><span data-stu-id="9b103-117">Property</span></span>     | <span data-ttu-id="9b103-118">类型</span><span class="sxs-lookup"><span data-stu-id="9b103-118">Type</span></span>   |<span data-ttu-id="9b103-119">说明</span><span class="sxs-lookup"><span data-stu-id="9b103-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b103-120">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="9b103-120">formulaHidden</span></span>|<span data-ttu-id="9b103-121">boolean</span><span class="sxs-lookup"><span data-stu-id="9b103-121">boolean</span></span>|<span data-ttu-id="9b103-p101">表示 Excel 是否隐藏区域中的单元格公式。指示整个区域不具有统一公式隐藏设置的空值。</span><span class="sxs-lookup"><span data-stu-id="9b103-p101">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="9b103-124">已锁定</span><span class="sxs-lookup"><span data-stu-id="9b103-124">locked</span></span>|<span data-ttu-id="9b103-125">boolean</span><span class="sxs-lookup"><span data-stu-id="9b103-125">boolean</span></span>|<span data-ttu-id="9b103-p102">指示 Excel 是否锁定对象中的单元格。指示整个区域不具有统一锁定设置的空值。</span><span class="sxs-lookup"><span data-stu-id="9b103-p102">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b103-128">关系</span><span class="sxs-lookup"><span data-stu-id="9b103-128">Relationships</span></span>
<span data-ttu-id="9b103-129">无</span><span class="sxs-lookup"><span data-stu-id="9b103-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9b103-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9b103-130">JSON representation</span></span>

<span data-ttu-id="9b103-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9b103-131">Here is a JSON representation of the resource.</span></span>

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
