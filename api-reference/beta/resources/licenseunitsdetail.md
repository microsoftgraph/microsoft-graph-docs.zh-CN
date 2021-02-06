---
title: licenseUnitsDetail 资源类型
description: '**subscribedSku** 实体的 prepaidUnits 属性为 **licenseUnitsDetail** 类型。'
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: krbain
ms.openlocfilehash: 3d4925c2acea0216e16283eaa8f779cb556e0857
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132431"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="ec899-103">licenseUnitsDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="ec899-103">licenseUnitsDetail resource type</span></span>

<span data-ttu-id="ec899-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec899-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec899-105">**subscribedSku** 实体的 [prepaidUnits](subscribedsku.md) 属性为 **licenseUnitsDetail** 类型。</span><span class="sxs-lookup"><span data-stu-id="ec899-105">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="ec899-106">属性</span><span class="sxs-lookup"><span data-stu-id="ec899-106">Properties</span></span>
| <span data-ttu-id="ec899-107">属性</span><span class="sxs-lookup"><span data-stu-id="ec899-107">Property</span></span>     | <span data-ttu-id="ec899-108">类型</span><span class="sxs-lookup"><span data-stu-id="ec899-108">Type</span></span>   |<span data-ttu-id="ec899-109">说明</span><span class="sxs-lookup"><span data-stu-id="ec899-109">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="ec899-110">已启用</span><span class="sxs-lookup"><span data-stu-id="ec899-110">enabled</span></span>|<span data-ttu-id="ec899-111">Int32</span><span class="sxs-lookup"><span data-stu-id="ec899-111">Int32</span></span>| <span data-ttu-id="ec899-112">启用的单位数。</span><span class="sxs-lookup"><span data-stu-id="ec899-112">The number of units that are enabled.</span></span> |
|<span data-ttu-id="ec899-113">已挂起</span><span class="sxs-lookup"><span data-stu-id="ec899-113">suspended</span></span>|<span data-ttu-id="ec899-114">Int32</span><span class="sxs-lookup"><span data-stu-id="ec899-114">Int32</span></span>| <span data-ttu-id="ec899-115">挂起的单位数。</span><span class="sxs-lookup"><span data-stu-id="ec899-115">The number of units that are suspended.</span></span> |
|<span data-ttu-id="ec899-116">警告</span><span class="sxs-lookup"><span data-stu-id="ec899-116">warning</span></span>|<span data-ttu-id="ec899-117">Int32</span><span class="sxs-lookup"><span data-stu-id="ec899-117">Int32</span></span>| <span data-ttu-id="ec899-118">警告状态的单位数。</span><span class="sxs-lookup"><span data-stu-id="ec899-118">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ec899-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ec899-119">JSON representation</span></span>

<span data-ttu-id="ec899-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ec899-120">Here is a JSON representation of the resource</span></span>

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


