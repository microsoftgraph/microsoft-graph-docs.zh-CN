---
title: licenseUnitsDetail 资源类型
description: subscribedSku 实体的 **prepaidUnits** 属性为 **licenseUnitsDetail** 类型。
ms.openlocfilehash: e8cf5253676dab8a4b31c3ab33faa0af3ddfd527
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007799"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="0625f-103">licenseUnitsDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="0625f-103">licenseUnitsDetail resource type</span></span>

<span data-ttu-id="0625f-104">[subscribedSku](subscribedsku.md) 实体的 **prepaidUnits** 属性为 **licenseUnitsDetail** 类型。</span><span class="sxs-lookup"><span data-stu-id="0625f-104">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="0625f-105">属性</span><span class="sxs-lookup"><span data-stu-id="0625f-105">Properties</span></span>
| <span data-ttu-id="0625f-106">属性</span><span class="sxs-lookup"><span data-stu-id="0625f-106">Property</span></span>     | <span data-ttu-id="0625f-107">类型</span><span class="sxs-lookup"><span data-stu-id="0625f-107">Type</span></span>   |<span data-ttu-id="0625f-108">说明</span><span class="sxs-lookup"><span data-stu-id="0625f-108">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="0625f-109">已启用</span><span class="sxs-lookup"><span data-stu-id="0625f-109">enabled</span></span>|<span data-ttu-id="0625f-110">Int32</span><span class="sxs-lookup"><span data-stu-id="0625f-110">Int32</span></span>| <span data-ttu-id="0625f-111">已启用的单元数。</span><span class="sxs-lookup"><span data-stu-id="0625f-111">The number of units that are enabled.</span></span> |
|<span data-ttu-id="0625f-112">suspended</span><span class="sxs-lookup"><span data-stu-id="0625f-112">suspended</span></span>|<span data-ttu-id="0625f-113">Int32</span><span class="sxs-lookup"><span data-stu-id="0625f-113">Int32</span></span>| <span data-ttu-id="0625f-114">已挂起的单元数。</span><span class="sxs-lookup"><span data-stu-id="0625f-114">The number of units that are suspended.</span></span> |
|<span data-ttu-id="0625f-115">warning</span><span class="sxs-lookup"><span data-stu-id="0625f-115">warning</span></span>|<span data-ttu-id="0625f-116">Int32</span><span class="sxs-lookup"><span data-stu-id="0625f-116">Int32</span></span>| <span data-ttu-id="0625f-117">处于警告状态的单元数。</span><span class="sxs-lookup"><span data-stu-id="0625f-117">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0625f-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0625f-118">JSON representation</span></span>

<span data-ttu-id="0625f-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0625f-119">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "licenseUnitsDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
