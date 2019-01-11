---
title: licenseUnitsDetail 资源类型
description: subscribedSku 实体的 **prepaidUnits** 属性为 **licenseUnitsDetail** 类型。
localization_priority: Normal
ms.openlocfilehash: d6fb464eaf9c1247d21ad9effb2b70c6bdaa1c3c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883508"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="bdd99-103">licenseUnitsDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="bdd99-103">licenseUnitsDetail resource type</span></span>

> <span data-ttu-id="bdd99-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bdd99-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bdd99-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bdd99-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bdd99-106">[subscribedSku](subscribedsku.md) 实体的 **prepaidUnits** 属性为 **licenseUnitsDetail** 类型。</span><span class="sxs-lookup"><span data-stu-id="bdd99-106">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="bdd99-107">属性</span><span class="sxs-lookup"><span data-stu-id="bdd99-107">Properties</span></span>
| <span data-ttu-id="bdd99-108">属性</span><span class="sxs-lookup"><span data-stu-id="bdd99-108">Property</span></span>     | <span data-ttu-id="bdd99-109">类型</span><span class="sxs-lookup"><span data-stu-id="bdd99-109">Type</span></span>   |<span data-ttu-id="bdd99-110">说明</span><span class="sxs-lookup"><span data-stu-id="bdd99-110">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="bdd99-111">已启用</span><span class="sxs-lookup"><span data-stu-id="bdd99-111">enabled</span></span>|<span data-ttu-id="bdd99-112">Int32</span><span class="sxs-lookup"><span data-stu-id="bdd99-112">Int32</span></span>| <span data-ttu-id="bdd99-113">已启用的单元数。</span><span class="sxs-lookup"><span data-stu-id="bdd99-113">The number of units that are enabled.</span></span> |
|<span data-ttu-id="bdd99-114">suspended</span><span class="sxs-lookup"><span data-stu-id="bdd99-114">suspended</span></span>|<span data-ttu-id="bdd99-115">Int32</span><span class="sxs-lookup"><span data-stu-id="bdd99-115">Int32</span></span>| <span data-ttu-id="bdd99-116">已挂起的单元数。</span><span class="sxs-lookup"><span data-stu-id="bdd99-116">The number of units that are suspended.</span></span> |
|<span data-ttu-id="bdd99-117">warning</span><span class="sxs-lookup"><span data-stu-id="bdd99-117">warning</span></span>|<span data-ttu-id="bdd99-118">Int32</span><span class="sxs-lookup"><span data-stu-id="bdd99-118">Int32</span></span>| <span data-ttu-id="bdd99-119">处于警告状态的单元数。</span><span class="sxs-lookup"><span data-stu-id="bdd99-119">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bdd99-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bdd99-120">JSON representation</span></span>

<span data-ttu-id="bdd99-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bdd99-121">Here is a JSON representation of the resource</span></span>

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
