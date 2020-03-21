---
title: 打印资源类型
description: 当附带通用打印订阅时，打印功能启用打印机的管理和 printServiceEndpoints 的发现，可用于管理通用打印中的打印机和打印作业。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 3ef5c05be520bb407f17d0af14bbd4355e736c62
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895636"
---
# <a name="print-resource-type"></a><span data-ttu-id="44a1e-103">打印资源类型</span><span class="sxs-lookup"><span data-stu-id="44a1e-103">print resource type</span></span>

<span data-ttu-id="44a1e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44a1e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44a1e-105">当附带通用打印订阅时，打印功能启用打印机的管理和[printServiceEndpoints](printserviceendpoint.md)的发现，可用于管理通用打印中的打印机和打印作业。</span><span class="sxs-lookup"><span data-stu-id="44a1e-105">When accompanied by a Universal Print subscription, the Print feature enables management of printers and discovery of [printServiceEndpoints](printserviceendpoint.md) that can be used to manage printers and print jobs within Universal Print.</span></span>

## <a name="methods"></a><span data-ttu-id="44a1e-106">方法</span><span class="sxs-lookup"><span data-stu-id="44a1e-106">Methods</span></span>
| <span data-ttu-id="44a1e-107">方法</span><span class="sxs-lookup"><span data-stu-id="44a1e-107">Method</span></span>       | <span data-ttu-id="44a1e-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="44a1e-108">Return Type</span></span> | <span data-ttu-id="44a1e-109">说明</span><span class="sxs-lookup"><span data-stu-id="44a1e-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="44a1e-110">列出连接器</span><span class="sxs-lookup"><span data-stu-id="44a1e-110">List connectors</span></span>](../api/print-list-connectors.md) | <span data-ttu-id="44a1e-111">[printConnector](printconnector.md)集合</span><span class="sxs-lookup"><span data-stu-id="44a1e-111">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="44a1e-112">获取打印连接器的列表。</span><span class="sxs-lookup"><span data-stu-id="44a1e-112">Get a list of print connectors.</span></span> |
| [<span data-ttu-id="44a1e-113">列出打印机</span><span class="sxs-lookup"><span data-stu-id="44a1e-113">List printers</span></span>](../api/print-list-printers.md) | <span data-ttu-id="44a1e-114">[打印机](printer.md)集合</span><span class="sxs-lookup"><span data-stu-id="44a1e-114">[printer](printer.md) collection</span></span> | <span data-ttu-id="44a1e-115">获取打印机的列表。</span><span class="sxs-lookup"><span data-stu-id="44a1e-115">Get a list of printers.</span></span> |
| [<span data-ttu-id="44a1e-116">列出 printerShares</span><span class="sxs-lookup"><span data-stu-id="44a1e-116">List printerShares</span></span>](../api/print-list-printershares.md) | <span data-ttu-id="44a1e-117">[printerShare](printershare.md)集合</span><span class="sxs-lookup"><span data-stu-id="44a1e-117">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="44a1e-118">获取打印机共享的列表。</span><span class="sxs-lookup"><span data-stu-id="44a1e-118">Get a list of printer shares.</span></span> |
| [<span data-ttu-id="44a1e-119">列出服务</span><span class="sxs-lookup"><span data-stu-id="44a1e-119">List services</span></span>](../api/print-list-services.md) | <span data-ttu-id="44a1e-120">[printService](printservice.md)集合</span><span class="sxs-lookup"><span data-stu-id="44a1e-120">[printService](printservice.md) collection</span></span> | <span data-ttu-id="44a1e-121">获取服务的列表。</span><span class="sxs-lookup"><span data-stu-id="44a1e-121">Get a list of services.</span></span> |
| [<span data-ttu-id="44a1e-122">创建 printerShare</span><span class="sxs-lookup"><span data-stu-id="44a1e-122">Create printerShare</span></span>](../api/print-post-printershares.md) | [<span data-ttu-id="44a1e-123">printerShare</span><span class="sxs-lookup"><span data-stu-id="44a1e-123">printerShare</span></span>](printershare.md) | <span data-ttu-id="44a1e-124">通过发布到**printerShares**集合创建新的打印机共享。</span><span class="sxs-lookup"><span data-stu-id="44a1e-124">Create a new printer share by posting to the **printerShares** collection.</span></span> |
| [<span data-ttu-id="44a1e-125">更新设置</span><span class="sxs-lookup"><span data-stu-id="44a1e-125">Update settings</span></span>](../api/print-update-settings.md) |  [<span data-ttu-id="44a1e-126">printSettings</span><span class="sxs-lookup"><span data-stu-id="44a1e-126">printSettings</span></span>](printsettings.md) | <span data-ttu-id="44a1e-127">更新通用打印服务的租户范围设置。</span><span class="sxs-lookup"><span data-stu-id="44a1e-127">Updates tenant-wide settings for the Universal Print service.</span></span> |

## <a name="properties"></a><span data-ttu-id="44a1e-128">属性</span><span class="sxs-lookup"><span data-stu-id="44a1e-128">Properties</span></span>
| <span data-ttu-id="44a1e-129">属性</span><span class="sxs-lookup"><span data-stu-id="44a1e-129">Property</span></span>     | <span data-ttu-id="44a1e-130">类型</span><span class="sxs-lookup"><span data-stu-id="44a1e-130">Type</span></span>        | <span data-ttu-id="44a1e-131">说明</span><span class="sxs-lookup"><span data-stu-id="44a1e-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="44a1e-132">settings</span><span class="sxs-lookup"><span data-stu-id="44a1e-132">settings</span></span>|[<span data-ttu-id="44a1e-133">printSettings</span><span class="sxs-lookup"><span data-stu-id="44a1e-133">printSettings</span></span>](printsettings.md)|<span data-ttu-id="44a1e-134">通用打印服务的租户范围内的设置。</span><span class="sxs-lookup"><span data-stu-id="44a1e-134">Tenant-wide settings for the Universal Print service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="44a1e-135">关系</span><span class="sxs-lookup"><span data-stu-id="44a1e-135">Relationships</span></span>
| <span data-ttu-id="44a1e-136">关系</span><span class="sxs-lookup"><span data-stu-id="44a1e-136">Relationship</span></span> | <span data-ttu-id="44a1e-137">类型</span><span class="sxs-lookup"><span data-stu-id="44a1e-137">Type</span></span>        | <span data-ttu-id="44a1e-138">说明</span><span class="sxs-lookup"><span data-stu-id="44a1e-138">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="44a1e-139">服务行业</span><span class="sxs-lookup"><span data-stu-id="44a1e-139">services</span></span>|<span data-ttu-id="44a1e-140">[printService](printservice.md)集合</span><span class="sxs-lookup"><span data-stu-id="44a1e-140">[printService](printservice.md) collection</span></span>|<span data-ttu-id="44a1e-141">可用通用打印服务终结点的列表。</span><span class="sxs-lookup"><span data-stu-id="44a1e-141">The list of available Universal Print service endpoints.</span></span>|
|<span data-ttu-id="44a1e-142">台</span><span class="sxs-lookup"><span data-stu-id="44a1e-142">printers</span></span>|<span data-ttu-id="44a1e-143">[打印机](printer.md)集合</span><span class="sxs-lookup"><span data-stu-id="44a1e-143">[printer](printer.md) collection</span></span>|<span data-ttu-id="44a1e-144">在租户中注册的打印机的列表。</span><span class="sxs-lookup"><span data-stu-id="44a1e-144">The list of printers registered in the tenant.</span></span>|
|<span data-ttu-id="44a1e-145">printerShares</span><span class="sxs-lookup"><span data-stu-id="44a1e-145">printerShares</span></span>|<span data-ttu-id="44a1e-146">[printerShare](printershare.md)集合集合</span><span class="sxs-lookup"><span data-stu-id="44a1e-146">[printerShare](printershare.md) collection collection</span></span>|<span data-ttu-id="44a1e-147">在租户中注册的打印机共享的列表。</span><span class="sxs-lookup"><span data-stu-id="44a1e-147">The list of printer shares registered in the tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="44a1e-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="44a1e-148">JSON representation</span></span>

<span data-ttu-id="44a1e-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44a1e-149">The following is a JSON representation of the resource.</span></span>

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