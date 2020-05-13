---
title: 打印资源类型
description: 当附带通用打印订阅时，打印功能启用打印机的管理和 printServiceEndpoints 的发现，可用于管理通用打印中的打印机和打印作业。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: b0af3f7443b77920804f5868fe9ecc3f8b4cec41
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44217085"
---
# <a name="print-resource-type"></a><span data-ttu-id="ac77a-103">打印资源类型</span><span class="sxs-lookup"><span data-stu-id="ac77a-103">print resource type</span></span>

<span data-ttu-id="ac77a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac77a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac77a-105">当附带通用打印订阅时，打印功能启用打印机的管理和[printServiceEndpoints](printserviceendpoint.md)的发现，可用于管理通用打印中的打印机和打印作业。</span><span class="sxs-lookup"><span data-stu-id="ac77a-105">When accompanied by a Universal Print subscription, the Print feature enables management of printers and discovery of [printServiceEndpoints](printserviceendpoint.md) that can be used to manage printers and print jobs within Universal Print.</span></span>

## <a name="methods"></a><span data-ttu-id="ac77a-106">Methods</span><span class="sxs-lookup"><span data-stu-id="ac77a-106">Methods</span></span>
| <span data-ttu-id="ac77a-107">方法</span><span class="sxs-lookup"><span data-stu-id="ac77a-107">Method</span></span>       | <span data-ttu-id="ac77a-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="ac77a-108">Return Type</span></span> | <span data-ttu-id="ac77a-109">说明</span><span class="sxs-lookup"><span data-stu-id="ac77a-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ac77a-110">列出连接器</span><span class="sxs-lookup"><span data-stu-id="ac77a-110">List connectors</span></span>](../api/print-list-connectors.md) | <span data-ttu-id="ac77a-111">[printConnector](printconnector.md)集合</span><span class="sxs-lookup"><span data-stu-id="ac77a-111">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="ac77a-112">获取打印连接器的列表。</span><span class="sxs-lookup"><span data-stu-id="ac77a-112">Get a list of print connectors.</span></span> |
| [<span data-ttu-id="ac77a-113">列出打印机</span><span class="sxs-lookup"><span data-stu-id="ac77a-113">List printers</span></span>](../api/print-list-printers.md) | <span data-ttu-id="ac77a-114">[打印机](printer.md)集合</span><span class="sxs-lookup"><span data-stu-id="ac77a-114">[printer](printer.md) collection</span></span> | <span data-ttu-id="ac77a-115">获取打印机的列表。</span><span class="sxs-lookup"><span data-stu-id="ac77a-115">Get a list of printers.</span></span> |
| [<span data-ttu-id="ac77a-116">列出共享</span><span class="sxs-lookup"><span data-stu-id="ac77a-116">List shares</span></span>](../api/print-list-shares.md) | <span data-ttu-id="ac77a-117">[printerShare](printershare.md)集合</span><span class="sxs-lookup"><span data-stu-id="ac77a-117">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="ac77a-118">获取打印机共享的列表。</span><span class="sxs-lookup"><span data-stu-id="ac77a-118">Get a list of printer shares.</span></span> |
| [<span data-ttu-id="ac77a-119">列出服务</span><span class="sxs-lookup"><span data-stu-id="ac77a-119">List services</span></span>](../api/print-list-services.md) | <span data-ttu-id="ac77a-120">[printService](printservice.md)集合</span><span class="sxs-lookup"><span data-stu-id="ac77a-120">[printService](printservice.md) collection</span></span> | <span data-ttu-id="ac77a-121">获取服务的列表。</span><span class="sxs-lookup"><span data-stu-id="ac77a-121">Get a list of services.</span></span> |
| [<span data-ttu-id="ac77a-122">创建 printerShare</span><span class="sxs-lookup"><span data-stu-id="ac77a-122">Create printerShare</span></span>](../api/print-post-shares.md) | [<span data-ttu-id="ac77a-123">printerShare</span><span class="sxs-lookup"><span data-stu-id="ac77a-123">printerShare</span></span>](printershare.md) | <span data-ttu-id="ac77a-124">通过发布到**共享**集合创建新的打印机共享。</span><span class="sxs-lookup"><span data-stu-id="ac77a-124">Create a new printer share by posting to the **shares** collection.</span></span> |
| [<span data-ttu-id="ac77a-125">更新设置</span><span class="sxs-lookup"><span data-stu-id="ac77a-125">Update settings</span></span>](../api/print-update-settings.md) |  [<span data-ttu-id="ac77a-126">printSettings</span><span class="sxs-lookup"><span data-stu-id="ac77a-126">printSettings</span></span>](printsettings.md) | <span data-ttu-id="ac77a-127">更新通用打印服务的租户范围设置。</span><span class="sxs-lookup"><span data-stu-id="ac77a-127">Updates tenant-wide settings for the Universal Print service.</span></span> |

## <a name="properties"></a><span data-ttu-id="ac77a-128">属性</span><span class="sxs-lookup"><span data-stu-id="ac77a-128">Properties</span></span>
| <span data-ttu-id="ac77a-129">属性</span><span class="sxs-lookup"><span data-stu-id="ac77a-129">Property</span></span>     | <span data-ttu-id="ac77a-130">类型</span><span class="sxs-lookup"><span data-stu-id="ac77a-130">Type</span></span>        | <span data-ttu-id="ac77a-131">说明</span><span class="sxs-lookup"><span data-stu-id="ac77a-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ac77a-132">settings</span><span class="sxs-lookup"><span data-stu-id="ac77a-132">settings</span></span>|[<span data-ttu-id="ac77a-133">printSettings</span><span class="sxs-lookup"><span data-stu-id="ac77a-133">printSettings</span></span>](printsettings.md)|<span data-ttu-id="ac77a-134">通用打印服务的租户范围内的设置。</span><span class="sxs-lookup"><span data-stu-id="ac77a-134">Tenant-wide settings for the Universal Print service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac77a-135">关系</span><span class="sxs-lookup"><span data-stu-id="ac77a-135">Relationships</span></span>
| <span data-ttu-id="ac77a-136">关系</span><span class="sxs-lookup"><span data-stu-id="ac77a-136">Relationship</span></span> | <span data-ttu-id="ac77a-137">类型</span><span class="sxs-lookup"><span data-stu-id="ac77a-137">Type</span></span>        | <span data-ttu-id="ac77a-138">说明</span><span class="sxs-lookup"><span data-stu-id="ac77a-138">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ac77a-139">服务行业</span><span class="sxs-lookup"><span data-stu-id="ac77a-139">services</span></span>|<span data-ttu-id="ac77a-140">[printService](printservice.md)集合</span><span class="sxs-lookup"><span data-stu-id="ac77a-140">[printService](printservice.md) collection</span></span>|<span data-ttu-id="ac77a-141">可用通用打印服务终结点的列表。</span><span class="sxs-lookup"><span data-stu-id="ac77a-141">The list of available Universal Print service endpoints.</span></span>|
|<span data-ttu-id="ac77a-142">台</span><span class="sxs-lookup"><span data-stu-id="ac77a-142">printers</span></span>|<span data-ttu-id="ac77a-143">[打印机](printer.md)集合</span><span class="sxs-lookup"><span data-stu-id="ac77a-143">[printer](printer.md) collection</span></span>|<span data-ttu-id="ac77a-144">在租户中注册的打印机的列表。</span><span class="sxs-lookup"><span data-stu-id="ac77a-144">The list of printers registered in the tenant.</span></span>|
|<span data-ttu-id="ac77a-145">shares</span><span class="sxs-lookup"><span data-stu-id="ac77a-145">shares</span></span>|<span data-ttu-id="ac77a-146">[printerShare](printershare.md)集合</span><span class="sxs-lookup"><span data-stu-id="ac77a-146">[printerShare](printershare.md) collection</span></span>|<span data-ttu-id="ac77a-147">在租户中注册的打印机共享的列表。</span><span class="sxs-lookup"><span data-stu-id="ac77a-147">The list of printer shares registered in the tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ac77a-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ac77a-148">JSON representation</span></span>

<span data-ttu-id="ac77a-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ac77a-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.print",
  "keyProperty": "settings"
}-->

```json
{
  "settings": {"@odata.type": "microsoft.graph.printSettings"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "print resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [ 
    "Error: Resource print has documented navigation properties, but we thought it was a complex type!",
    "Resource print has documented navigation properties, but we thought it was a complex type!"
}-->