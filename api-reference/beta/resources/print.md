---
title: 打印资源类型
description: 当附带通用打印订阅时，打印功能启用打印机的管理和 printServiceEndpoints 的发现，可用于管理通用打印中的打印机和打印作业。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 309b7c8e62b94703bb00e21fb8c8ed2a2e917efe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985886"
---
# <a name="print-resource-type"></a><span data-ttu-id="572bb-103">打印资源类型</span><span class="sxs-lookup"><span data-stu-id="572bb-103">print resource type</span></span>

<span data-ttu-id="572bb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="572bb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="572bb-105">当附带通用打印订阅时，打印功能启用打印机的管理和 [printServiceEndpoints](printserviceendpoint.md) 的发现，可用于管理通用打印中的打印机和打印作业。</span><span class="sxs-lookup"><span data-stu-id="572bb-105">When accompanied by a Universal Print subscription, the Print feature enables management of printers and discovery of [printServiceEndpoints](printserviceendpoint.md) that can be used to manage printers and print jobs within Universal Print.</span></span>

## <a name="methods"></a><span data-ttu-id="572bb-106">方法</span><span class="sxs-lookup"><span data-stu-id="572bb-106">Methods</span></span>
| <span data-ttu-id="572bb-107">方法</span><span class="sxs-lookup"><span data-stu-id="572bb-107">Method</span></span>       | <span data-ttu-id="572bb-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="572bb-108">Return Type</span></span> | <span data-ttu-id="572bb-109">说明</span><span class="sxs-lookup"><span data-stu-id="572bb-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="572bb-110">List connectors</span><span class="sxs-lookup"><span data-stu-id="572bb-110">List connectors</span></span>](../api/print-list-connectors.md) | <span data-ttu-id="572bb-111">[printConnector](printconnector.md) 集合</span><span class="sxs-lookup"><span data-stu-id="572bb-111">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="572bb-112">获取打印连接器的列表。</span><span class="sxs-lookup"><span data-stu-id="572bb-112">Get a list of print connectors.</span></span> |
| [<span data-ttu-id="572bb-113">列出打印机</span><span class="sxs-lookup"><span data-stu-id="572bb-113">List printers</span></span>](../api/print-list-printers.md) | <span data-ttu-id="572bb-114">[打印机](printer.md) 集合</span><span class="sxs-lookup"><span data-stu-id="572bb-114">[printer](printer.md) collection</span></span> | <span data-ttu-id="572bb-115">获取打印机的列表。</span><span class="sxs-lookup"><span data-stu-id="572bb-115">Get a list of printers.</span></span> |
| [<span data-ttu-id="572bb-116">列出共享项</span><span class="sxs-lookup"><span data-stu-id="572bb-116">List shares</span></span>](../api/print-list-shares.md) | <span data-ttu-id="572bb-117">[printerShare](printershare.md) 集合</span><span class="sxs-lookup"><span data-stu-id="572bb-117">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="572bb-118">获取打印机共享的列表。</span><span class="sxs-lookup"><span data-stu-id="572bb-118">Get a list of printer shares.</span></span> |
| [<span data-ttu-id="572bb-119">列出服务</span><span class="sxs-lookup"><span data-stu-id="572bb-119">List services</span></span>](../api/print-list-services.md) | <span data-ttu-id="572bb-120">[printService](printservice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="572bb-120">[printService](printservice.md) collection</span></span> | <span data-ttu-id="572bb-121">获取服务的列表。</span><span class="sxs-lookup"><span data-stu-id="572bb-121">Get a list of services.</span></span> |
| [<span data-ttu-id="572bb-122">创建 printerShare</span><span class="sxs-lookup"><span data-stu-id="572bb-122">Create printerShare</span></span>](../api/print-post-shares.md) | [<span data-ttu-id="572bb-123">printerShare</span><span class="sxs-lookup"><span data-stu-id="572bb-123">printerShare</span></span>](printershare.md) | <span data-ttu-id="572bb-124">通过发布到 **共享** 集合创建新的打印机共享。</span><span class="sxs-lookup"><span data-stu-id="572bb-124">Create a new printer share by posting to the **shares** collection.</span></span> |
| [<span data-ttu-id="572bb-125">创建打印机</span><span class="sxs-lookup"><span data-stu-id="572bb-125">Create printer</span></span>](../api/printer-create.md) | [<span data-ttu-id="572bb-126">printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="572bb-126">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="572bb-127">创建 (注册) 具有通用打印的新打印机。</span><span class="sxs-lookup"><span data-stu-id="572bb-127">Create (register) a new printer with Universal Print.</span></span> |
| [<span data-ttu-id="572bb-128">更新设置</span><span class="sxs-lookup"><span data-stu-id="572bb-128">Update settings</span></span>](../api/print-update-settings.md) |  [<span data-ttu-id="572bb-129">printSettings</span><span class="sxs-lookup"><span data-stu-id="572bb-129">printSettings</span></span>](printsettings.md) | <span data-ttu-id="572bb-130">更新通用打印服务的租户范围设置。</span><span class="sxs-lookup"><span data-stu-id="572bb-130">Updates tenant-wide settings for the Universal Print service.</span></span> |
| [<span data-ttu-id="572bb-131">List taskDefinitions</span><span class="sxs-lookup"><span data-stu-id="572bb-131">List taskDefinitions</span></span>](../api/print-list-taskdefinitions.md) | <span data-ttu-id="572bb-132">[printTaskDefinition](printtaskdefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="572bb-132">[printTaskDefinition](printtaskdefinition.md) collection</span></span> | <span data-ttu-id="572bb-133">获取在通用打印中创建的 printTaskDefinitions 的租户范围列表。</span><span class="sxs-lookup"><span data-stu-id="572bb-133">Get a tenant-wide list of printTaskDefinitions created within Universal Print.</span></span> |
| [<span data-ttu-id="572bb-134">Create taskDefinition</span><span class="sxs-lookup"><span data-stu-id="572bb-134">Create taskDefinition</span></span>](../api/print-post-taskdefinitions.md) | [<span data-ttu-id="572bb-135">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="572bb-135">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="572bb-136">创建新的 printTaskDefinition。</span><span class="sxs-lookup"><span data-stu-id="572bb-136">Create a new printTaskDefinition.</span></span> |
| [<span data-ttu-id="572bb-137">Update taskDefinition</span><span class="sxs-lookup"><span data-stu-id="572bb-137">Update taskDefinition</span></span>](../api/print-update-taskdefinition.md) | [<span data-ttu-id="572bb-138">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="572bb-138">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="572bb-139">更新 printTaskDefinition。</span><span class="sxs-lookup"><span data-stu-id="572bb-139">Update a printTaskDefinition.</span></span> |
| [<span data-ttu-id="572bb-140">Delete taskDefinition</span><span class="sxs-lookup"><span data-stu-id="572bb-140">Delete taskDefinition</span></span>](../api/print-delete-taskdefinition.md) | <span data-ttu-id="572bb-141">无</span><span class="sxs-lookup"><span data-stu-id="572bb-141">None</span></span> | <span data-ttu-id="572bb-142">删除 printTaskDefinition。</span><span class="sxs-lookup"><span data-stu-id="572bb-142">Delete a printTaskDefinition.</span></span> |

## <a name="properties"></a><span data-ttu-id="572bb-143">属性</span><span class="sxs-lookup"><span data-stu-id="572bb-143">Properties</span></span>
| <span data-ttu-id="572bb-144">属性</span><span class="sxs-lookup"><span data-stu-id="572bb-144">Property</span></span>     | <span data-ttu-id="572bb-145">类型</span><span class="sxs-lookup"><span data-stu-id="572bb-145">Type</span></span>        | <span data-ttu-id="572bb-146">说明</span><span class="sxs-lookup"><span data-stu-id="572bb-146">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="572bb-147">settings</span><span class="sxs-lookup"><span data-stu-id="572bb-147">settings</span></span>|[<span data-ttu-id="572bb-148">printSettings</span><span class="sxs-lookup"><span data-stu-id="572bb-148">printSettings</span></span>](printsettings.md)|<span data-ttu-id="572bb-149">通用打印服务的租户范围内的设置。</span><span class="sxs-lookup"><span data-stu-id="572bb-149">Tenant-wide settings for the Universal Print service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="572bb-150">关系</span><span class="sxs-lookup"><span data-stu-id="572bb-150">Relationships</span></span>
| <span data-ttu-id="572bb-151">关系</span><span class="sxs-lookup"><span data-stu-id="572bb-151">Relationship</span></span> | <span data-ttu-id="572bb-152">类型</span><span class="sxs-lookup"><span data-stu-id="572bb-152">Type</span></span>        | <span data-ttu-id="572bb-153">说明</span><span class="sxs-lookup"><span data-stu-id="572bb-153">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="572bb-154">服务行业</span><span class="sxs-lookup"><span data-stu-id="572bb-154">services</span></span>|<span data-ttu-id="572bb-155">[printService](printservice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="572bb-155">[printService](printservice.md) collection</span></span>|<span data-ttu-id="572bb-156">可用通用打印服务终结点的列表。</span><span class="sxs-lookup"><span data-stu-id="572bb-156">The list of available Universal Print service endpoints.</span></span>|
|<span data-ttu-id="572bb-157">台</span><span class="sxs-lookup"><span data-stu-id="572bb-157">printers</span></span>|<span data-ttu-id="572bb-158">[打印机](printer.md) 集合</span><span class="sxs-lookup"><span data-stu-id="572bb-158">[printer](printer.md) collection</span></span>|<span data-ttu-id="572bb-159">在租户中注册的打印机的列表。</span><span class="sxs-lookup"><span data-stu-id="572bb-159">The list of printers registered in the tenant.</span></span>|
|<span data-ttu-id="572bb-160">shares</span><span class="sxs-lookup"><span data-stu-id="572bb-160">shares</span></span>|<span data-ttu-id="572bb-161">[printerShare](printershare.md) 集合</span><span class="sxs-lookup"><span data-stu-id="572bb-161">[printerShare](printershare.md) collection</span></span>|<span data-ttu-id="572bb-162">在租户中注册的打印机共享的列表。</span><span class="sxs-lookup"><span data-stu-id="572bb-162">The list of printer shares registered in the tenant.</span></span>|
|<span data-ttu-id="572bb-163">插槽</span><span class="sxs-lookup"><span data-stu-id="572bb-163">connectors</span></span>|<span data-ttu-id="572bb-164">[printConnector](printconnector.md) 集合</span><span class="sxs-lookup"><span data-stu-id="572bb-164">[printConnector](printconnector.md) collection</span></span>|<span data-ttu-id="572bb-165">可用打印连接器的列表。</span><span class="sxs-lookup"><span data-stu-id="572bb-165">The list of available print connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="572bb-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="572bb-166">JSON representation</span></span>

<span data-ttu-id="572bb-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="572bb-167">The following is a JSON representation of the resource.</span></span>

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


