---
title: licenseUnitsDetail 资源类型
description: '**subscribedSku** 实体的 prepaidUnits 属性为 **licenseUnitsDetail** 类型。'
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4de4d89b5abec06abc6d2f8bfa4f78c22abe4ca0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447575"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="fe700-103">licenseUnitsDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="fe700-103">licenseUnitsDetail resource type</span></span>

<span data-ttu-id="fe700-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="fe700-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fe700-105">**subscribedSku** 实体的 [prepaidUnits](subscribedsku.md) 属性为 **licenseUnitsDetail** 类型。</span><span class="sxs-lookup"><span data-stu-id="fe700-105">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="fe700-106">属性</span><span class="sxs-lookup"><span data-stu-id="fe700-106">Properties</span></span>
| <span data-ttu-id="fe700-107">属性</span><span class="sxs-lookup"><span data-stu-id="fe700-107">Property</span></span>     | <span data-ttu-id="fe700-108">类型</span><span class="sxs-lookup"><span data-stu-id="fe700-108">Type</span></span>   |<span data-ttu-id="fe700-109">说明</span><span class="sxs-lookup"><span data-stu-id="fe700-109">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="fe700-110">已启用</span><span class="sxs-lookup"><span data-stu-id="fe700-110">enabled</span></span>|<span data-ttu-id="fe700-111">Int32</span><span class="sxs-lookup"><span data-stu-id="fe700-111">Int32</span></span>| <span data-ttu-id="fe700-112">启用的单位数。</span><span class="sxs-lookup"><span data-stu-id="fe700-112">The number of units that are enabled.</span></span> |
|<span data-ttu-id="fe700-113">已挂起</span><span class="sxs-lookup"><span data-stu-id="fe700-113">suspended</span></span>|<span data-ttu-id="fe700-114">Int32</span><span class="sxs-lookup"><span data-stu-id="fe700-114">Int32</span></span>| <span data-ttu-id="fe700-115">挂起的单位数。</span><span class="sxs-lookup"><span data-stu-id="fe700-115">The number of units that are suspended.</span></span> |
|<span data-ttu-id="fe700-116">警告</span><span class="sxs-lookup"><span data-stu-id="fe700-116">warning</span></span>|<span data-ttu-id="fe700-117">Int32</span><span class="sxs-lookup"><span data-stu-id="fe700-117">Int32</span></span>| <span data-ttu-id="fe700-118">处于警告状态的单位数。</span><span class="sxs-lookup"><span data-stu-id="fe700-118">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fe700-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fe700-119">JSON representation</span></span>

<span data-ttu-id="fe700-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe700-120">Here is a JSON representation of the resource</span></span>

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
