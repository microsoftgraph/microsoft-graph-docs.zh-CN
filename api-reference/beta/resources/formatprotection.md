---
title: FormatProtection 资源类型
description: 表示对 range 对象的格式保护。
ms.openlocfilehash: 5f2a4968b018a952b24bb18a75a4f6d5aff55b00
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046075"
---
# <a name="formatprotection-resource-type"></a><span data-ttu-id="f8250-103">FormatProtection 资源类型</span><span class="sxs-lookup"><span data-stu-id="f8250-103">FormatProtection resource type</span></span>

> <span data-ttu-id="f8250-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f8250-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8250-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f8250-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f8250-106">表示对 range 对象的格式保护。</span><span class="sxs-lookup"><span data-stu-id="f8250-106">Represents the format protection of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="f8250-107">方法</span><span class="sxs-lookup"><span data-stu-id="f8250-107">Methods</span></span>

| <span data-ttu-id="f8250-108">方法</span><span class="sxs-lookup"><span data-stu-id="f8250-108">Method</span></span>           | <span data-ttu-id="f8250-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="f8250-109">Return Type</span></span>    |<span data-ttu-id="f8250-110">说明</span><span class="sxs-lookup"><span data-stu-id="f8250-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f8250-111">获取 FormatProtection</span><span class="sxs-lookup"><span data-stu-id="f8250-111">Get FormatProtection</span></span>](../api/formatprotection-get.md) | [<span data-ttu-id="f8250-112">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="f8250-112">FormatProtection</span></span>](formatprotection.md) |<span data-ttu-id="f8250-113">读取 formatProtection 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f8250-113">Read properties and relationships of formatProtection object.</span></span>|
|[<span data-ttu-id="f8250-114">Update</span><span class="sxs-lookup"><span data-stu-id="f8250-114">Update</span></span>](../api/formatprotection-update.md) | [<span data-ttu-id="f8250-115">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="f8250-115">FormatProtection</span></span>](formatprotection.md)  |<span data-ttu-id="f8250-116">更新 FormatProtection 对象。</span><span class="sxs-lookup"><span data-stu-id="f8250-116">Update FormatProtection object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f8250-117">属性</span><span class="sxs-lookup"><span data-stu-id="f8250-117">Properties</span></span>
| <span data-ttu-id="f8250-118">属性</span><span class="sxs-lookup"><span data-stu-id="f8250-118">Property</span></span>     | <span data-ttu-id="f8250-119">类型</span><span class="sxs-lookup"><span data-stu-id="f8250-119">Type</span></span>   |<span data-ttu-id="f8250-120">说明</span><span class="sxs-lookup"><span data-stu-id="f8250-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f8250-121">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="f8250-121">formulaHidden</span></span>|<span data-ttu-id="f8250-122">boolean</span><span class="sxs-lookup"><span data-stu-id="f8250-122">boolean</span></span>|<span data-ttu-id="f8250-p102">表示 Excel 是否隐藏区域中的单元格公式。指示整个区域不具有统一公式隐藏设置的空值。</span><span class="sxs-lookup"><span data-stu-id="f8250-p102">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="f8250-125">已锁定</span><span class="sxs-lookup"><span data-stu-id="f8250-125">locked</span></span>|<span data-ttu-id="f8250-126">boolean</span><span class="sxs-lookup"><span data-stu-id="f8250-126">boolean</span></span>|<span data-ttu-id="f8250-p103">指示 Excel 是否锁定对象中的单元格。指示整个区域不具有统一锁定设置的空值。</span><span class="sxs-lookup"><span data-stu-id="f8250-p103">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8250-129">Relationships</span><span class="sxs-lookup"><span data-stu-id="f8250-129">Relationships</span></span>
<span data-ttu-id="f8250-130">无</span><span class="sxs-lookup"><span data-stu-id="f8250-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f8250-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f8250-131">JSON representation</span></span>

<span data-ttu-id="f8250-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f8250-132">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "FormatProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->