---
title: 打印资源类型
description: 当随附通用打印订阅时，打印功能允许管理打印机和发现可用于在通用打印中管理打印机和打印作业的 printServiceEndpoints。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 0604044824d153c9e6d39586c2ca58ee9ca893ea
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292250"
---
# <a name="print-resource-type"></a><span data-ttu-id="1be19-103">打印资源类型</span><span class="sxs-lookup"><span data-stu-id="1be19-103">print resource type</span></span>

<span data-ttu-id="1be19-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1be19-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1be19-105">当随附通用打印订阅时，打印功能允许管理打印机和发现可用于在通用打印中管理打印机和打印作业的[printServiceEndpoints。](printserviceendpoint.md)</span><span class="sxs-lookup"><span data-stu-id="1be19-105">When accompanied by a Universal Print subscription, the Print feature enables management of printers and discovery of [printServiceEndpoints](printserviceendpoint.md) that can be used to manage printers and print jobs within Universal Print.</span></span>

## <a name="methods"></a><span data-ttu-id="1be19-106">方法</span><span class="sxs-lookup"><span data-stu-id="1be19-106">Methods</span></span>
| <span data-ttu-id="1be19-107">方法</span><span class="sxs-lookup"><span data-stu-id="1be19-107">Method</span></span>       | <span data-ttu-id="1be19-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="1be19-108">Return Type</span></span> | <span data-ttu-id="1be19-109">说明</span><span class="sxs-lookup"><span data-stu-id="1be19-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1be19-110">List connectors</span><span class="sxs-lookup"><span data-stu-id="1be19-110">List connectors</span></span>](../api/print-list-connectors.md) | <span data-ttu-id="1be19-111">[printConnector](printconnector.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1be19-111">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="1be19-112">获取打印连接器的列表。</span><span class="sxs-lookup"><span data-stu-id="1be19-112">Get a list of print connectors.</span></span> |
| [<span data-ttu-id="1be19-113">列出打印机</span><span class="sxs-lookup"><span data-stu-id="1be19-113">List printers</span></span>](../api/print-list-printers.md) | <span data-ttu-id="1be19-114">[打印机](printer.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1be19-114">[printer](printer.md) collection</span></span> | <span data-ttu-id="1be19-115">获取打印机列表。</span><span class="sxs-lookup"><span data-stu-id="1be19-115">Get a list of printers.</span></span> |
| [<span data-ttu-id="1be19-116">列出共享项</span><span class="sxs-lookup"><span data-stu-id="1be19-116">List shares</span></span>](../api/print-list-shares.md) | <span data-ttu-id="1be19-117">[printerShare](printershare.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1be19-117">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="1be19-118">获取打印机共享的列表。</span><span class="sxs-lookup"><span data-stu-id="1be19-118">Get a list of printer shares.</span></span> |
| [<span data-ttu-id="1be19-119">列出服务</span><span class="sxs-lookup"><span data-stu-id="1be19-119">List services</span></span>](../api/print-list-services.md) | <span data-ttu-id="1be19-120">[printService](printservice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1be19-120">[printService](printservice.md) collection</span></span> | <span data-ttu-id="1be19-121">获取服务列表。</span><span class="sxs-lookup"><span data-stu-id="1be19-121">Get a list of services.</span></span> |
| [<span data-ttu-id="1be19-122">创建 printerShare</span><span class="sxs-lookup"><span data-stu-id="1be19-122">Create printerShare</span></span>](../api/print-post-shares.md) | [<span data-ttu-id="1be19-123">printerShare</span><span class="sxs-lookup"><span data-stu-id="1be19-123">printerShare</span></span>](printershare.md) | <span data-ttu-id="1be19-124">通过发布到共享集合创建新的 **打印机** 共享。</span><span class="sxs-lookup"><span data-stu-id="1be19-124">Create a new printer share by posting to the **shares** collection.</span></span> |
| [<span data-ttu-id="1be19-125">创建打印机</span><span class="sxs-lookup"><span data-stu-id="1be19-125">Create printer</span></span>](../api/printer-create.md) | [<span data-ttu-id="1be19-126">printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="1be19-126">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="1be19-127">创建 (通用) 新打印机上注册。</span><span class="sxs-lookup"><span data-stu-id="1be19-127">Create (register) a new printer with Universal Print.</span></span> |
| [<span data-ttu-id="1be19-128">更新设置</span><span class="sxs-lookup"><span data-stu-id="1be19-128">Update settings</span></span>](../api/print-update-settings.md) |  [<span data-ttu-id="1be19-129">printSettings</span><span class="sxs-lookup"><span data-stu-id="1be19-129">printSettings</span></span>](printsettings.md) | <span data-ttu-id="1be19-130">更新通用打印服务的租户范围设置。</span><span class="sxs-lookup"><span data-stu-id="1be19-130">Updates tenant-wide settings for the Universal Print service.</span></span> |
| [<span data-ttu-id="1be19-131">List taskDefinitions</span><span class="sxs-lookup"><span data-stu-id="1be19-131">List taskDefinitions</span></span>](../api/print-list-taskdefinitions.md) | <span data-ttu-id="1be19-132">[printTaskDefinition](printtaskdefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1be19-132">[printTaskDefinition](printtaskdefinition.md) collection</span></span> | <span data-ttu-id="1be19-133">获取在通用打印中创建的 printTaskDefinitions 的租户范围列表。</span><span class="sxs-lookup"><span data-stu-id="1be19-133">Get a tenant-wide list of printTaskDefinitions created within Universal Print.</span></span> |
| [<span data-ttu-id="1be19-134">Create taskDefinition</span><span class="sxs-lookup"><span data-stu-id="1be19-134">Create taskDefinition</span></span>](../api/print-post-taskdefinitions.md) | [<span data-ttu-id="1be19-135">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="1be19-135">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="1be19-136">创建新的 printTaskDefinition。</span><span class="sxs-lookup"><span data-stu-id="1be19-136">Create a new printTaskDefinition.</span></span> |
| [<span data-ttu-id="1be19-137">Update taskDefinition</span><span class="sxs-lookup"><span data-stu-id="1be19-137">Update taskDefinition</span></span>](../api/print-update-taskdefinition.md) | [<span data-ttu-id="1be19-138">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="1be19-138">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="1be19-139">更新 printTaskDefinition。</span><span class="sxs-lookup"><span data-stu-id="1be19-139">Update a printTaskDefinition.</span></span> |
| [<span data-ttu-id="1be19-140">Delete taskDefinition</span><span class="sxs-lookup"><span data-stu-id="1be19-140">Delete taskDefinition</span></span>](../api/print-delete-taskdefinition.md) | <span data-ttu-id="1be19-141">无</span><span class="sxs-lookup"><span data-stu-id="1be19-141">None</span></span> | <span data-ttu-id="1be19-142">删除 printTaskDefinition。</span><span class="sxs-lookup"><span data-stu-id="1be19-142">Delete a printTaskDefinition.</span></span> |

## <a name="properties"></a><span data-ttu-id="1be19-143">属性</span><span class="sxs-lookup"><span data-stu-id="1be19-143">Properties</span></span>
| <span data-ttu-id="1be19-144">属性</span><span class="sxs-lookup"><span data-stu-id="1be19-144">Property</span></span>     | <span data-ttu-id="1be19-145">类型</span><span class="sxs-lookup"><span data-stu-id="1be19-145">Type</span></span>        | <span data-ttu-id="1be19-146">说明</span><span class="sxs-lookup"><span data-stu-id="1be19-146">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1be19-147">settings</span><span class="sxs-lookup"><span data-stu-id="1be19-147">settings</span></span>|[<span data-ttu-id="1be19-148">printSettings</span><span class="sxs-lookup"><span data-stu-id="1be19-148">printSettings</span></span>](printsettings.md)|<span data-ttu-id="1be19-149">通用打印服务的租户范围设置。</span><span class="sxs-lookup"><span data-stu-id="1be19-149">Tenant-wide settings for the Universal Print service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1be19-150">关系</span><span class="sxs-lookup"><span data-stu-id="1be19-150">Relationships</span></span>
| <span data-ttu-id="1be19-151">关系</span><span class="sxs-lookup"><span data-stu-id="1be19-151">Relationship</span></span> | <span data-ttu-id="1be19-152">类型</span><span class="sxs-lookup"><span data-stu-id="1be19-152">Type</span></span>        | <span data-ttu-id="1be19-153">说明</span><span class="sxs-lookup"><span data-stu-id="1be19-153">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1be19-154">服务</span><span class="sxs-lookup"><span data-stu-id="1be19-154">services</span></span>|<span data-ttu-id="1be19-155">[printService](printservice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1be19-155">[printService](printservice.md) collection</span></span>|<span data-ttu-id="1be19-156">可用通用打印服务终结点的列表。</span><span class="sxs-lookup"><span data-stu-id="1be19-156">The list of available Universal Print service endpoints.</span></span>|
|<span data-ttu-id="1be19-157">打印机</span><span class="sxs-lookup"><span data-stu-id="1be19-157">printers</span></span>|<span data-ttu-id="1be19-158">[打印机](printer.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1be19-158">[printer](printer.md) collection</span></span>|<span data-ttu-id="1be19-159">在租户中注册的打印机列表。</span><span class="sxs-lookup"><span data-stu-id="1be19-159">The list of printers registered in the tenant.</span></span>|
|<span data-ttu-id="1be19-160">shares</span><span class="sxs-lookup"><span data-stu-id="1be19-160">shares</span></span>|<span data-ttu-id="1be19-161">[printerShare](printershare.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1be19-161">[printerShare](printershare.md) collection</span></span>|<span data-ttu-id="1be19-162">租户中注册的打印机共享列表。</span><span class="sxs-lookup"><span data-stu-id="1be19-162">The list of printer shares registered in the tenant.</span></span>|
|<span data-ttu-id="1be19-163">连接器</span><span class="sxs-lookup"><span data-stu-id="1be19-163">connectors</span></span>|<span data-ttu-id="1be19-164">[printConnector](printconnector.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1be19-164">[printConnector](printconnector.md) collection</span></span>|<span data-ttu-id="1be19-165">可用打印连接器的列表。</span><span class="sxs-lookup"><span data-stu-id="1be19-165">The list of available print connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1be19-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1be19-166">JSON representation</span></span>

<span data-ttu-id="1be19-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1be19-167">The following is a JSON representation of the resource.</span></span>

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
  ]
}-->


