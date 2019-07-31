---
title: licenseUnitsDetail 资源类型
description: '**subscribedSku** 实体的 prepaidUnits 属性为 **licenseUnitsDetail** 类型。'
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4482f9661b41981717422c7c874319fbca7be23d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966966"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="c038e-103">licenseUnitsDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="c038e-103">licenseUnitsDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c038e-104">**subscribedSku** 实体的 [prepaidUnits](subscribedsku.md) 属性为 **licenseUnitsDetail** 类型。</span><span class="sxs-lookup"><span data-stu-id="c038e-104">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="c038e-105">属性</span><span class="sxs-lookup"><span data-stu-id="c038e-105">Properties</span></span>
| <span data-ttu-id="c038e-106">属性</span><span class="sxs-lookup"><span data-stu-id="c038e-106">Property</span></span>     | <span data-ttu-id="c038e-107">类型</span><span class="sxs-lookup"><span data-stu-id="c038e-107">Type</span></span>   |<span data-ttu-id="c038e-108">说明</span><span class="sxs-lookup"><span data-stu-id="c038e-108">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="c038e-109">已启用</span><span class="sxs-lookup"><span data-stu-id="c038e-109">enabled</span></span>|<span data-ttu-id="c038e-110">Int32</span><span class="sxs-lookup"><span data-stu-id="c038e-110">Int32</span></span>| <span data-ttu-id="c038e-111">启用的单位数。</span><span class="sxs-lookup"><span data-stu-id="c038e-111">The number of units that are enabled.</span></span> |
|<span data-ttu-id="c038e-112">已挂起</span><span class="sxs-lookup"><span data-stu-id="c038e-112">suspended</span></span>|<span data-ttu-id="c038e-113">Int32</span><span class="sxs-lookup"><span data-stu-id="c038e-113">Int32</span></span>| <span data-ttu-id="c038e-114">挂起的单位数。</span><span class="sxs-lookup"><span data-stu-id="c038e-114">The number of units that are suspended.</span></span> |
|<span data-ttu-id="c038e-115">警告</span><span class="sxs-lookup"><span data-stu-id="c038e-115">warning</span></span>|<span data-ttu-id="c038e-116">Int32</span><span class="sxs-lookup"><span data-stu-id="c038e-116">Int32</span></span>| <span data-ttu-id="c038e-117">处于警告状态的单位数。</span><span class="sxs-lookup"><span data-stu-id="c038e-117">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c038e-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c038e-118">JSON representation</span></span>

<span data-ttu-id="c038e-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c038e-119">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseUnitsDetail"
}-->

```json
{
  "enabled": 1024,
  "suspended": 1024,
  "warning": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "licenseUnitsDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
