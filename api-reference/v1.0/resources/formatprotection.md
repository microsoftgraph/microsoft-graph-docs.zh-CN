---
title: FormatProtection 资源类型
description: 表示对范围对象的格式保护。
localization_priority: Normal
ms.openlocfilehash: e4c32c8be8f6ef3aeaaf763ee88998bcbe235503
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542051"
---
# <a name="formatprotection-resource-type"></a><span data-ttu-id="f8ec2-103">FormatProtection 资源类型</span><span class="sxs-lookup"><span data-stu-id="f8ec2-103">FormatProtection resource type</span></span>

<span data-ttu-id="f8ec2-104">表示对范围对象的格式保护。</span><span class="sxs-lookup"><span data-stu-id="f8ec2-104">Represents the format protection of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="f8ec2-105">方法</span><span class="sxs-lookup"><span data-stu-id="f8ec2-105">Methods</span></span>

| <span data-ttu-id="f8ec2-106">方法</span><span class="sxs-lookup"><span data-stu-id="f8ec2-106">Method</span></span>           | <span data-ttu-id="f8ec2-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="f8ec2-107">Return Type</span></span>    |<span data-ttu-id="f8ec2-108">说明</span><span class="sxs-lookup"><span data-stu-id="f8ec2-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f8ec2-109">获取 FormatProtection</span><span class="sxs-lookup"><span data-stu-id="f8ec2-109">Get FormatProtection</span></span>](../api/formatprotection-get.md) | [<span data-ttu-id="f8ec2-110">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="f8ec2-110">FormatProtection</span></span>](formatprotection.md) |<span data-ttu-id="f8ec2-111">读取 formatProtection 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f8ec2-111">Read properties and relationships of formatProtection object.</span></span>|
|[<span data-ttu-id="f8ec2-112">更新</span><span class="sxs-lookup"><span data-stu-id="f8ec2-112">Update</span></span>](../api/formatprotection-update.md) | [<span data-ttu-id="f8ec2-113">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="f8ec2-113">FormatProtection</span></span>](formatprotection.md)  |<span data-ttu-id="f8ec2-114">更新 FormatProtection 对象。</span><span class="sxs-lookup"><span data-stu-id="f8ec2-114">Update FormatProtection object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f8ec2-115">属性</span><span class="sxs-lookup"><span data-stu-id="f8ec2-115">Properties</span></span>
| <span data-ttu-id="f8ec2-116">属性</span><span class="sxs-lookup"><span data-stu-id="f8ec2-116">Property</span></span>     | <span data-ttu-id="f8ec2-117">类型</span><span class="sxs-lookup"><span data-stu-id="f8ec2-117">Type</span></span>   |<span data-ttu-id="f8ec2-118">说明</span><span class="sxs-lookup"><span data-stu-id="f8ec2-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f8ec2-119">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="f8ec2-119">formulaHidden</span></span>|<span data-ttu-id="f8ec2-120">布尔</span><span class="sxs-lookup"><span data-stu-id="f8ec2-120">boolean</span></span>|<span data-ttu-id="f8ec2-p101">表示 Excel 是否隐藏区域中的单元格公式。指示整个区域不具有统一公式隐藏设置的空值。</span><span class="sxs-lookup"><span data-stu-id="f8ec2-p101">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="f8ec2-123">已锁定</span><span class="sxs-lookup"><span data-stu-id="f8ec2-123">locked</span></span>|<span data-ttu-id="f8ec2-124">boolean</span><span class="sxs-lookup"><span data-stu-id="f8ec2-124">boolean</span></span>|<span data-ttu-id="f8ec2-p102">指示 Excel 是否锁定对象中的单元格。指示整个区域不具有统一锁定设置的空值。</span><span class="sxs-lookup"><span data-stu-id="f8ec2-p102">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8ec2-127">关系</span><span class="sxs-lookup"><span data-stu-id="f8ec2-127">Relationships</span></span>
<span data-ttu-id="f8ec2-128">无</span><span class="sxs-lookup"><span data-stu-id="f8ec2-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f8ec2-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f8ec2-129">JSON representation</span></span>

<span data-ttu-id="f8ec2-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f8ec2-130">Here is a JSON representation of the resource.</span></span>

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
