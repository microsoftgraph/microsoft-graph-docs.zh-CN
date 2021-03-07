---
title: printerBase 资源类型
description: 表示打印机和打印机共享的基本类型
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 515c14bb4de7352a8c17cffdacbd7a4c9091fc70
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516946"
---
# <a name="printerbase-resource-type"></a><span data-ttu-id="7436b-103">printerBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="7436b-103">printerBase resource type</span></span>

<span data-ttu-id="7436b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7436b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="7436b-105">表示打印机和[printerShare](printer.md) [](printerShare.md)实体类型的基本类型。</span><span class="sxs-lookup"><span data-stu-id="7436b-105">Represents a base type for [printer](printer.md) and [printerShare](printerShare.md) entity types.</span></span>

## <a name="properties"></a><span data-ttu-id="7436b-106">属性</span><span class="sxs-lookup"><span data-stu-id="7436b-106">Properties</span></span>
|<span data-ttu-id="7436b-107">属性</span><span class="sxs-lookup"><span data-stu-id="7436b-107">Property</span></span>|<span data-ttu-id="7436b-108">类型</span><span class="sxs-lookup"><span data-stu-id="7436b-108">Type</span></span>|<span data-ttu-id="7436b-109">Description</span><span class="sxs-lookup"><span data-stu-id="7436b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7436b-110">capabilities</span><span class="sxs-lookup"><span data-stu-id="7436b-110">capabilities</span></span>|[<span data-ttu-id="7436b-111">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="7436b-111">printerCapabilities</span></span>](printercapabilities.md)|<span data-ttu-id="7436b-112">printer/printerShare 的功能。</span><span class="sxs-lookup"><span data-stu-id="7436b-112">The capabilities of the printer/printerShare.</span></span>|
|<span data-ttu-id="7436b-113">defaults</span><span class="sxs-lookup"><span data-stu-id="7436b-113">defaults</span></span>|[<span data-ttu-id="7436b-114">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="7436b-114">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="7436b-115">printer/printerShare 的默认打印设置。</span><span class="sxs-lookup"><span data-stu-id="7436b-115">The default print settings of printer/printerShare.</span></span>|
|<span data-ttu-id="7436b-116">displayName</span><span class="sxs-lookup"><span data-stu-id="7436b-116">displayName</span></span>|<span data-ttu-id="7436b-117">String</span><span class="sxs-lookup"><span data-stu-id="7436b-117">String</span></span>|<span data-ttu-id="7436b-118">printer/printerShare 的名称。</span><span class="sxs-lookup"><span data-stu-id="7436b-118">The name of the printer/printerShare.</span></span>|
|<span data-ttu-id="7436b-119">id</span><span class="sxs-lookup"><span data-stu-id="7436b-119">id</span></span>|<span data-ttu-id="7436b-120">String</span><span class="sxs-lookup"><span data-stu-id="7436b-120">String</span></span>|<span data-ttu-id="7436b-121">标识符。</span><span class="sxs-lookup"><span data-stu-id="7436b-121">The identifier.</span></span>|
|<span data-ttu-id="7436b-122">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="7436b-122">isAcceptingJobs</span></span>|<span data-ttu-id="7436b-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="7436b-123">Boolean</span></span>|<span data-ttu-id="7436b-124">打印机/打印机共享当前是否接受新的打印作业。</span><span class="sxs-lookup"><span data-stu-id="7436b-124">Whether the printer/printerShare is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="7436b-125">位置</span><span class="sxs-lookup"><span data-stu-id="7436b-125">location</span></span>|[<span data-ttu-id="7436b-126">printerLocation</span><span class="sxs-lookup"><span data-stu-id="7436b-126">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="7436b-127">打印机/printerShare 的物理和/或组织位置。</span><span class="sxs-lookup"><span data-stu-id="7436b-127">The physical and/or organizational location of the printer/printerShare.</span></span>|
|<span data-ttu-id="7436b-128">manufacturer</span><span class="sxs-lookup"><span data-stu-id="7436b-128">manufacturer</span></span>|<span data-ttu-id="7436b-129">String</span><span class="sxs-lookup"><span data-stu-id="7436b-129">String</span></span>|<span data-ttu-id="7436b-130">打印机/printerShare 的制造商。</span><span class="sxs-lookup"><span data-stu-id="7436b-130">The manufacturer of the printer/printerShare.</span></span>|
|<span data-ttu-id="7436b-131">model</span><span class="sxs-lookup"><span data-stu-id="7436b-131">model</span></span>|<span data-ttu-id="7436b-132">String</span><span class="sxs-lookup"><span data-stu-id="7436b-132">String</span></span>|<span data-ttu-id="7436b-133">打印机/printerShare 的模型名称。</span><span class="sxs-lookup"><span data-stu-id="7436b-133">The model name of the printer/printerShare.</span></span>|
|<span data-ttu-id="7436b-134">状态</span><span class="sxs-lookup"><span data-stu-id="7436b-134">status</span></span>|[<span data-ttu-id="7436b-135">printerStatus</span><span class="sxs-lookup"><span data-stu-id="7436b-135">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="7436b-136">打印机/printerShare 的处理状态，包括任何错误。</span><span class="sxs-lookup"><span data-stu-id="7436b-136">The processing status of the printer/printerShare, including any errors.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7436b-137">关系</span><span class="sxs-lookup"><span data-stu-id="7436b-137">Relationships</span></span>
|<span data-ttu-id="7436b-138">关系</span><span class="sxs-lookup"><span data-stu-id="7436b-138">Relationship</span></span>|<span data-ttu-id="7436b-139">类型</span><span class="sxs-lookup"><span data-stu-id="7436b-139">Type</span></span>|<span data-ttu-id="7436b-140">Description</span><span class="sxs-lookup"><span data-stu-id="7436b-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7436b-141">jobs</span><span class="sxs-lookup"><span data-stu-id="7436b-141">jobs</span></span>|<span data-ttu-id="7436b-142">[printJob](printjob.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7436b-142">[printJob](printjob.md) collection</span></span>|<span data-ttu-id="7436b-143">由打印机/printerShare 排入打印队列的作业列表。</span><span class="sxs-lookup"><span data-stu-id="7436b-143">The list of jobs that are queued for printing by the printer/printerShare.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7436b-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7436b-144">JSON representation</span></span>
<span data-ttu-id="7436b-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7436b-145">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printerBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerBase",
  "id": "String (identifier)",
  "displayName": "String",
  "manufacturer": "String",
  "model": "String",
  "isAcceptingJobs": "Boolean",
  "defaults": {
    "@odata.type": "microsoft.graph.printerDefaults"
  },
  "location": {
    "@odata.type": "microsoft.graph.printerLocation"
  },
  "capabilities": {
    "@odata.type": "microsoft.graph.printerCapabilities"
  },
  "status": {
    "@odata.type": "microsoft.graph.printerStatus"
  }
}
```

