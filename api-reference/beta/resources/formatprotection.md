---
title: FormatProtection 资源类型
description: 表示对范围对象的格式保护。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ruoyingl
ms.openlocfilehash: cbad1af0eea639b73e06d5678a2293d744964975
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809556"
---
# <a name="formatprotection-resource-type"></a><span data-ttu-id="07bca-103">FormatProtection 资源类型</span><span class="sxs-lookup"><span data-stu-id="07bca-103">FormatProtection resource type</span></span>

<span data-ttu-id="07bca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07bca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07bca-105">表示对范围对象的格式保护。</span><span class="sxs-lookup"><span data-stu-id="07bca-105">Represents the format protection of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="07bca-106">方法</span><span class="sxs-lookup"><span data-stu-id="07bca-106">Methods</span></span>

| <span data-ttu-id="07bca-107">方法</span><span class="sxs-lookup"><span data-stu-id="07bca-107">Method</span></span>           | <span data-ttu-id="07bca-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="07bca-108">Return Type</span></span>    |<span data-ttu-id="07bca-109">说明</span><span class="sxs-lookup"><span data-stu-id="07bca-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="07bca-110">获取 FormatProtection</span><span class="sxs-lookup"><span data-stu-id="07bca-110">Get FormatProtection</span></span>](../api/formatprotection-get.md) | [<span data-ttu-id="07bca-111">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="07bca-111">FormatProtection</span></span>](formatprotection.md) |<span data-ttu-id="07bca-112">读取 formatProtection 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="07bca-112">Read properties and relationships of formatProtection object.</span></span>|
|[<span data-ttu-id="07bca-113">更新</span><span class="sxs-lookup"><span data-stu-id="07bca-113">Update</span></span>](../api/formatprotection-update.md) | [<span data-ttu-id="07bca-114">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="07bca-114">FormatProtection</span></span>](formatprotection.md)  |<span data-ttu-id="07bca-115">更新 FormatProtection 对象。</span><span class="sxs-lookup"><span data-stu-id="07bca-115">Update FormatProtection object.</span></span> |

## <a name="properties"></a><span data-ttu-id="07bca-116">属性</span><span class="sxs-lookup"><span data-stu-id="07bca-116">Properties</span></span>
| <span data-ttu-id="07bca-117">属性</span><span class="sxs-lookup"><span data-stu-id="07bca-117">Property</span></span>     | <span data-ttu-id="07bca-118">类型</span><span class="sxs-lookup"><span data-stu-id="07bca-118">Type</span></span>   |<span data-ttu-id="07bca-119">说明</span><span class="sxs-lookup"><span data-stu-id="07bca-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07bca-120">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="07bca-120">formulaHidden</span></span>|<span data-ttu-id="07bca-121">boolean</span><span class="sxs-lookup"><span data-stu-id="07bca-121">boolean</span></span>|<span data-ttu-id="07bca-p101">表示 Excel 是否隐藏区域中的单元格公式。指示整个区域不具有统一公式隐藏设置的空值。</span><span class="sxs-lookup"><span data-stu-id="07bca-p101">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="07bca-124">已锁定</span><span class="sxs-lookup"><span data-stu-id="07bca-124">locked</span></span>|<span data-ttu-id="07bca-125">boolean</span><span class="sxs-lookup"><span data-stu-id="07bca-125">boolean</span></span>|<span data-ttu-id="07bca-p102">指示 Excel 是否锁定对象中的单元格。指示整个区域不具有统一锁定设置的空值。</span><span class="sxs-lookup"><span data-stu-id="07bca-p102">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07bca-128">关系</span><span class="sxs-lookup"><span data-stu-id="07bca-128">Relationships</span></span>
<span data-ttu-id="07bca-129">无</span><span class="sxs-lookup"><span data-stu-id="07bca-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="07bca-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="07bca-130">JSON representation</span></span>

<span data-ttu-id="07bca-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07bca-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.formatProtection"
}-->

```json
{
  "formulaHidden": true,
  "locked": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "FormatProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
