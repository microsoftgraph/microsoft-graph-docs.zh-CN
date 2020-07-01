---
title: 打印资源类型
description: 当附带通用打印订阅时，打印功能启用打印机的管理和 printServiceEndpoints 的发现，可用于管理通用打印中的打印机和打印作业。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 551fa42736d6fa275a8f998274a6fccf55ac00b7
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006973"
---
# <a name="print-resource-type"></a><span data-ttu-id="52d27-103">打印资源类型</span><span class="sxs-lookup"><span data-stu-id="52d27-103">print resource type</span></span>

<span data-ttu-id="52d27-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52d27-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52d27-105">当附带通用打印订阅时，打印功能启用打印机的管理和[printServiceEndpoints](printserviceendpoint.md)的发现，可用于管理通用打印中的打印机和打印作业。</span><span class="sxs-lookup"><span data-stu-id="52d27-105">When accompanied by a Universal Print subscription, the Print feature enables management of printers and discovery of [printServiceEndpoints](printserviceendpoint.md) that can be used to manage printers and print jobs within Universal Print.</span></span>

## <a name="methods"></a><span data-ttu-id="52d27-106">方法</span><span class="sxs-lookup"><span data-stu-id="52d27-106">Methods</span></span>
| <span data-ttu-id="52d27-107">方法</span><span class="sxs-lookup"><span data-stu-id="52d27-107">Method</span></span>       | <span data-ttu-id="52d27-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="52d27-108">Return Type</span></span> | <span data-ttu-id="52d27-109">说明</span><span class="sxs-lookup"><span data-stu-id="52d27-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="52d27-110">列出连接器</span><span class="sxs-lookup"><span data-stu-id="52d27-110">List connectors</span></span>](../api/print-list-connectors.md) | <span data-ttu-id="52d27-111">[printConnector](printconnector.md)集合</span><span class="sxs-lookup"><span data-stu-id="52d27-111">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="52d27-112">获取打印连接器的列表。</span><span class="sxs-lookup"><span data-stu-id="52d27-112">Get a list of print connectors.</span></span> |
| [<span data-ttu-id="52d27-113">列出打印机</span><span class="sxs-lookup"><span data-stu-id="52d27-113">List printers</span></span>](../api/print-list-printers.md) | <span data-ttu-id="52d27-114">[打印机](printer.md)集合</span><span class="sxs-lookup"><span data-stu-id="52d27-114">[printer](printer.md) collection</span></span> | <span data-ttu-id="52d27-115">获取打印机的列表。</span><span class="sxs-lookup"><span data-stu-id="52d27-115">Get a list of printers.</span></span> |
| [<span data-ttu-id="52d27-116">列出共享</span><span class="sxs-lookup"><span data-stu-id="52d27-116">List shares</span></span>](../api/print-list-shares.md) | <span data-ttu-id="52d27-117">[printerShare](printershare.md)集合</span><span class="sxs-lookup"><span data-stu-id="52d27-117">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="52d27-118">获取打印机共享的列表。</span><span class="sxs-lookup"><span data-stu-id="52d27-118">Get a list of printer shares.</span></span> |
| [<span data-ttu-id="52d27-119">列出服务</span><span class="sxs-lookup"><span data-stu-id="52d27-119">List services</span></span>](../api/print-list-services.md) | <span data-ttu-id="52d27-120">[printService](printservice.md)集合</span><span class="sxs-lookup"><span data-stu-id="52d27-120">[printService](printservice.md) collection</span></span> | <span data-ttu-id="52d27-121">获取服务的列表。</span><span class="sxs-lookup"><span data-stu-id="52d27-121">Get a list of services.</span></span> |
| [<span data-ttu-id="52d27-122">创建 printerShare</span><span class="sxs-lookup"><span data-stu-id="52d27-122">Create printerShare</span></span>](../api/print-post-shares.md) | [<span data-ttu-id="52d27-123">printerShare</span><span class="sxs-lookup"><span data-stu-id="52d27-123">printerShare</span></span>](printershare.md) | <span data-ttu-id="52d27-124">通过发布到**共享**集合创建新的打印机共享。</span><span class="sxs-lookup"><span data-stu-id="52d27-124">Create a new printer share by posting to the **shares** collection.</span></span> |
| [<span data-ttu-id="52d27-125">创建打印机</span><span class="sxs-lookup"><span data-stu-id="52d27-125">Create printer</span></span>](../api/printer-create.md) | [<span data-ttu-id="52d27-126">printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="52d27-126">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="52d27-127">创建（注册）具有通用打印的新打印机。</span><span class="sxs-lookup"><span data-stu-id="52d27-127">Create (register) a new printer with Universal Print.</span></span> |
| [<span data-ttu-id="52d27-128">更新设置</span><span class="sxs-lookup"><span data-stu-id="52d27-128">Update settings</span></span>](../api/print-update-settings.md) |  [<span data-ttu-id="52d27-129">printSettings</span><span class="sxs-lookup"><span data-stu-id="52d27-129">printSettings</span></span>](printsettings.md) | <span data-ttu-id="52d27-130">更新通用打印服务的租户范围设置。</span><span class="sxs-lookup"><span data-stu-id="52d27-130">Updates tenant-wide settings for the Universal Print service.</span></span> |

## <a name="properties"></a><span data-ttu-id="52d27-131">属性</span><span class="sxs-lookup"><span data-stu-id="52d27-131">Properties</span></span>
| <span data-ttu-id="52d27-132">属性</span><span class="sxs-lookup"><span data-stu-id="52d27-132">Property</span></span>     | <span data-ttu-id="52d27-133">类型</span><span class="sxs-lookup"><span data-stu-id="52d27-133">Type</span></span>        | <span data-ttu-id="52d27-134">说明</span><span class="sxs-lookup"><span data-stu-id="52d27-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="52d27-135">settings</span><span class="sxs-lookup"><span data-stu-id="52d27-135">settings</span></span>|[<span data-ttu-id="52d27-136">printSettings</span><span class="sxs-lookup"><span data-stu-id="52d27-136">printSettings</span></span>](printsettings.md)|<span data-ttu-id="52d27-137">通用打印服务的租户范围内的设置。</span><span class="sxs-lookup"><span data-stu-id="52d27-137">Tenant-wide settings for the Universal Print service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52d27-138">关系</span><span class="sxs-lookup"><span data-stu-id="52d27-138">Relationships</span></span>
| <span data-ttu-id="52d27-139">关系</span><span class="sxs-lookup"><span data-stu-id="52d27-139">Relationship</span></span> | <span data-ttu-id="52d27-140">类型</span><span class="sxs-lookup"><span data-stu-id="52d27-140">Type</span></span>        | <span data-ttu-id="52d27-141">说明</span><span class="sxs-lookup"><span data-stu-id="52d27-141">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="52d27-142">服务行业</span><span class="sxs-lookup"><span data-stu-id="52d27-142">services</span></span>|<span data-ttu-id="52d27-143">[printService](printservice.md)集合</span><span class="sxs-lookup"><span data-stu-id="52d27-143">[printService](printservice.md) collection</span></span>|<span data-ttu-id="52d27-144">可用通用打印服务终结点的列表。</span><span class="sxs-lookup"><span data-stu-id="52d27-144">The list of available Universal Print service endpoints.</span></span>|
|<span data-ttu-id="52d27-145">台</span><span class="sxs-lookup"><span data-stu-id="52d27-145">printers</span></span>|<span data-ttu-id="52d27-146">[打印机](printer.md)集合</span><span class="sxs-lookup"><span data-stu-id="52d27-146">[printer](printer.md) collection</span></span>|<span data-ttu-id="52d27-147">在租户中注册的打印机的列表。</span><span class="sxs-lookup"><span data-stu-id="52d27-147">The list of printers registered in the tenant.</span></span>|
|<span data-ttu-id="52d27-148">shares</span><span class="sxs-lookup"><span data-stu-id="52d27-148">shares</span></span>|<span data-ttu-id="52d27-149">[printerShare](printershare.md)集合</span><span class="sxs-lookup"><span data-stu-id="52d27-149">[printerShare](printershare.md) collection</span></span>|<span data-ttu-id="52d27-150">在租户中注册的打印机共享的列表。</span><span class="sxs-lookup"><span data-stu-id="52d27-150">The list of printer shares registered in the tenant.</span></span>|
|<span data-ttu-id="52d27-151">插槽</span><span class="sxs-lookup"><span data-stu-id="52d27-151">connectors</span></span>|<span data-ttu-id="52d27-152">[printConnector](printconnector.md)集合</span><span class="sxs-lookup"><span data-stu-id="52d27-152">[printConnector](printconnector.md) collection</span></span>|<span data-ttu-id="52d27-153">可用打印连接器的列表。</span><span class="sxs-lookup"><span data-stu-id="52d27-153">The list of available print connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="52d27-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="52d27-154">JSON representation</span></span>

<span data-ttu-id="52d27-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52d27-155">The following is a JSON representation of the resource.</span></span>

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
