---
title: 打印机资源类型
description: 表示已向通用打印服务注册的物理打印机设备。 打印机资源可用于管理打印作业、打印机设置、打印机元数据和注册状态。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 2f1decf04f48f7ee8dc074997e6d503130bc74bc
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848617"
---
# <a name="printer-resource-type"></a><span data-ttu-id="c3866-104">打印机资源类型</span><span class="sxs-lookup"><span data-stu-id="c3866-104">printer resource type</span></span>

<span data-ttu-id="c3866-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3866-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3866-106">表示已向通用打印服务注册的打印机设备。</span><span class="sxs-lookup"><span data-stu-id="c3866-106">Represents a printer device that has been registered with the Universal Print service.</span></span> <span data-ttu-id="c3866-107">打印机资源可用于管理打印作业、打印机设置、打印机元数据和注册状态。</span><span class="sxs-lookup"><span data-stu-id="c3866-107">Printer resources can be used to manage print jobs, printer settings, printer metadata and registration status.</span></span>

## <a name="methods"></a><span data-ttu-id="c3866-108">方法</span><span class="sxs-lookup"><span data-stu-id="c3866-108">Methods</span></span>

| <span data-ttu-id="c3866-109">方法</span><span class="sxs-lookup"><span data-stu-id="c3866-109">Method</span></span>       | <span data-ttu-id="c3866-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="c3866-110">Return Type</span></span> | <span data-ttu-id="c3866-111">说明</span><span class="sxs-lookup"><span data-stu-id="c3866-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c3866-112">创建</span><span class="sxs-lookup"><span data-stu-id="c3866-112">Create</span></span>](../api/printer-create.md) | [<span data-ttu-id="c3866-113">printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="c3866-113">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="c3866-114">创建 (注册) 具有通用打印的新打印机。</span><span class="sxs-lookup"><span data-stu-id="c3866-114">Create (register) a new printer with Universal Print.</span></span> |
| [<span data-ttu-id="c3866-115">获取</span><span class="sxs-lookup"><span data-stu-id="c3866-115">Get</span></span>](../api/printer-get.md) | [<span data-ttu-id="c3866-116">印刷</span><span class="sxs-lookup"><span data-stu-id="c3866-116">printer</span></span>](printer.md) | <span data-ttu-id="c3866-117">读取 printer 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c3866-117">Read the properties and relationships of the printer object.</span></span> |
| [<span data-ttu-id="c3866-118">更新</span><span class="sxs-lookup"><span data-stu-id="c3866-118">Update</span></span>](../api/printer-update.md) | [<span data-ttu-id="c3866-119">印刷</span><span class="sxs-lookup"><span data-stu-id="c3866-119">printer</span></span>](printer.md) | <span data-ttu-id="c3866-120">更新 printer 对象。</span><span class="sxs-lookup"><span data-stu-id="c3866-120">Update the printer object.</span></span> |
| [<span data-ttu-id="c3866-121">删除</span><span class="sxs-lookup"><span data-stu-id="c3866-121">Delete</span></span>](../api/printer-delete.md) | <span data-ttu-id="c3866-122">无</span><span class="sxs-lookup"><span data-stu-id="c3866-122">None</span></span> | <span data-ttu-id="c3866-123">从通用打印服务注销物理打印机。</span><span class="sxs-lookup"><span data-stu-id="c3866-123">Unregister the physical printer from the Universal Print service.</span></span> |
| [<span data-ttu-id="c3866-124">restoreFactoryDefaults</span><span class="sxs-lookup"><span data-stu-id="c3866-124">restoreFactoryDefaults</span></span>](../api/printer-restorefactorydefaults.md) | <span data-ttu-id="c3866-125">无</span><span class="sxs-lookup"><span data-stu-id="c3866-125">None</span></span> | <span data-ttu-id="c3866-126">将打印机的默认设置还原为制造商指定的值。</span><span class="sxs-lookup"><span data-stu-id="c3866-126">Restore a printer's default settings to the values specified by the manufacturer.</span></span> |
| [<span data-ttu-id="c3866-127">列出作业</span><span class="sxs-lookup"><span data-stu-id="c3866-127">List jobs</span></span>](../api/printer-list-jobs.md) | <span data-ttu-id="c3866-128">[printJob](printjob.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c3866-128">[printJob](printjob.md) collection</span></span> | <span data-ttu-id="c3866-129">获取排队等待打印机处理的打印作业的列表。</span><span class="sxs-lookup"><span data-stu-id="c3866-129">Get a list of print jobs that are queued for processing by the printer.</span></span> |
| [<span data-ttu-id="c3866-130">创建作业</span><span class="sxs-lookup"><span data-stu-id="c3866-130">Create job</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="c3866-131">printJob</span><span class="sxs-lookup"><span data-stu-id="c3866-131">printJob</span></span>](printjob.md) | <span data-ttu-id="c3866-132">为打印机创建一个新的打印作业。</span><span class="sxs-lookup"><span data-stu-id="c3866-132">Create a new print job for the printer.</span></span> <span data-ttu-id="c3866-133">若要开始打印作业，请使用 [start](../api/printjob-start.md)。</span><span class="sxs-lookup"><span data-stu-id="c3866-133">To start printing the job, use [start](../api/printjob-start.md).</span></span> |
| [<span data-ttu-id="c3866-134">List connectors</span><span class="sxs-lookup"><span data-stu-id="c3866-134">List connectors</span></span>](../api/printer-list-connectors.md) | <span data-ttu-id="c3866-135">[printConnector](printconnector.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c3866-135">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="c3866-136">获取此打印机关联的连接器的列表。</span><span class="sxs-lookup"><span data-stu-id="c3866-136">Get a list of connectors that this printer is associated with.</span></span> |
| [<span data-ttu-id="c3866-137">List taskTriggers</span><span class="sxs-lookup"><span data-stu-id="c3866-137">List taskTriggers</span></span>](../api/printer-list-tasktriggers.md) | <span data-ttu-id="c3866-138">无</span><span class="sxs-lookup"><span data-stu-id="c3866-138">None</span></span> | <span data-ttu-id="c3866-139">列出与此打印机关联的 [printTaskTriggers](printtasktrigger.md) 。</span><span class="sxs-lookup"><span data-stu-id="c3866-139">List [printTaskTriggers](printtasktrigger.md) associated with this printer.</span></span> |
| [<span data-ttu-id="c3866-140">Create taskTrigger</span><span class="sxs-lookup"><span data-stu-id="c3866-140">Create taskTrigger</span></span>](../api/printer-post-tasktriggers.md) | [<span data-ttu-id="c3866-141">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="c3866-141">printTaskTrigger</span></span>](printtasktrigger.md) | <span data-ttu-id="c3866-142">创建在打印事件发生时运行的 [printTaskTrigger](printtasktrigger.md) 。</span><span class="sxs-lookup"><span data-stu-id="c3866-142">Create a [printTaskTrigger](printtasktrigger.md) that runs when print events occur.</span></span> |
| [<span data-ttu-id="c3866-143">Delete taskTrigger</span><span class="sxs-lookup"><span data-stu-id="c3866-143">Delete taskTrigger</span></span>](../api/printer-delete-tasktrigger.md) | <span data-ttu-id="c3866-144">无</span><span class="sxs-lookup"><span data-stu-id="c3866-144">None</span></span> | <span data-ttu-id="c3866-145">删除与打印机关联的 [printTaskTrigger](printtasktrigger.md) 。</span><span class="sxs-lookup"><span data-stu-id="c3866-145">Delete a [printTaskTrigger](printtasktrigger.md) that is associated with the printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="c3866-146">属性</span><span class="sxs-lookup"><span data-stu-id="c3866-146">Properties</span></span>
| <span data-ttu-id="c3866-147">属性</span><span class="sxs-lookup"><span data-stu-id="c3866-147">Property</span></span>     | <span data-ttu-id="c3866-148">类型</span><span class="sxs-lookup"><span data-stu-id="c3866-148">Type</span></span>        | <span data-ttu-id="c3866-149">说明</span><span class="sxs-lookup"><span data-stu-id="c3866-149">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c3866-150">id</span><span class="sxs-lookup"><span data-stu-id="c3866-150">id</span></span>|<span data-ttu-id="c3866-151">String</span><span class="sxs-lookup"><span data-stu-id="c3866-151">String</span></span>|<span data-ttu-id="c3866-152">文档的标识符。</span><span class="sxs-lookup"><span data-stu-id="c3866-152">The document's identifier.</span></span> <span data-ttu-id="c3866-153">只读。</span><span class="sxs-lookup"><span data-stu-id="c3866-153">Read-only.</span></span>|
|<span data-ttu-id="c3866-154">displayName</span><span class="sxs-lookup"><span data-stu-id="c3866-154">displayName</span></span>|<span data-ttu-id="c3866-155">String</span><span class="sxs-lookup"><span data-stu-id="c3866-155">String</span></span>|<span data-ttu-id="c3866-156">打印机的名称。</span><span class="sxs-lookup"><span data-stu-id="c3866-156">The name of the printer.</span></span>|
|<span data-ttu-id="c3866-157">manufacturer</span><span class="sxs-lookup"><span data-stu-id="c3866-157">manufacturer</span></span>|<span data-ttu-id="c3866-158">String</span><span class="sxs-lookup"><span data-stu-id="c3866-158">String</span></span>|<span data-ttu-id="c3866-159">打印机报告的制造商。</span><span class="sxs-lookup"><span data-stu-id="c3866-159">The manufacturer reported by the printer.</span></span> <span data-ttu-id="c3866-160">只读。</span><span class="sxs-lookup"><span data-stu-id="c3866-160">Read-only.</span></span>|
|<span data-ttu-id="c3866-161">model</span><span class="sxs-lookup"><span data-stu-id="c3866-161">model</span></span>|<span data-ttu-id="c3866-162">String</span><span class="sxs-lookup"><span data-stu-id="c3866-162">String</span></span>|<span data-ttu-id="c3866-163">打印机报告的模型名称。</span><span class="sxs-lookup"><span data-stu-id="c3866-163">The model name reported by the printer.</span></span> <span data-ttu-id="c3866-164">只读。</span><span class="sxs-lookup"><span data-stu-id="c3866-164">Read-only.</span></span>|
|<span data-ttu-id="c3866-165">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="c3866-165">registeredDateTime</span></span>|<span data-ttu-id="c3866-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3866-166">DateTimeOffset</span></span>|<span data-ttu-id="c3866-167">注册打印机时的 DateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="c3866-167">The DateTimeOffset when the printer was registered.</span></span> <span data-ttu-id="c3866-168">只读。</span><span class="sxs-lookup"><span data-stu-id="c3866-168">Read-only.</span></span>|
|<span data-ttu-id="c3866-169">status</span><span class="sxs-lookup"><span data-stu-id="c3866-169">status</span></span>|[<span data-ttu-id="c3866-170">printerStatus</span><span class="sxs-lookup"><span data-stu-id="c3866-170">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="c3866-171">打印机的处理状态，包括任何错误。</span><span class="sxs-lookup"><span data-stu-id="c3866-171">The processing status of the printer, including any errors.</span></span> <span data-ttu-id="c3866-172">只读。</span><span class="sxs-lookup"><span data-stu-id="c3866-172">Read-only.</span></span>|
|<span data-ttu-id="c3866-173">isShared</span><span class="sxs-lookup"><span data-stu-id="c3866-173">isShared</span></span>|<span data-ttu-id="c3866-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3866-174">Boolean</span></span>|<span data-ttu-id="c3866-175">如果打印机是共享的，则为 True;否则为 false。</span><span class="sxs-lookup"><span data-stu-id="c3866-175">True if the printer is shared; false otherwise.</span></span> <span data-ttu-id="c3866-176">只读。</span><span class="sxs-lookup"><span data-stu-id="c3866-176">Read-only.</span></span>|
|<span data-ttu-id="c3866-177">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="c3866-177">isAcceptingJobs</span></span>|<span data-ttu-id="c3866-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3866-178">Boolean</span></span>|<span data-ttu-id="c3866-179">打印机当前是否正在接受新的打印作业。</span><span class="sxs-lookup"><span data-stu-id="c3866-179">Whether the printer is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="c3866-180">位置</span><span class="sxs-lookup"><span data-stu-id="c3866-180">location</span></span>|[<span data-ttu-id="c3866-181">printerLocation</span><span class="sxs-lookup"><span data-stu-id="c3866-181">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="c3866-182">打印机的物理和/或组织位置。</span><span class="sxs-lookup"><span data-stu-id="c3866-182">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="c3866-183">defaults</span><span class="sxs-lookup"><span data-stu-id="c3866-183">defaults</span></span>|[<span data-ttu-id="c3866-184">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="c3866-184">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="c3866-185">打印机的默认打印设置。</span><span class="sxs-lookup"><span data-stu-id="c3866-185">The printer's default print settings.</span></span>|
|<span data-ttu-id="c3866-186">capabilities</span><span class="sxs-lookup"><span data-stu-id="c3866-186">capabilities</span></span>|[<span data-ttu-id="c3866-187">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="c3866-187">printerCapabilities</span></span>](printercapabilities.md)|<span data-ttu-id="c3866-188">与此打印机共享相关联的打印机的功能。</span><span class="sxs-lookup"><span data-stu-id="c3866-188">The capabilities of the printer associated with this printer share.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3866-189">关系</span><span class="sxs-lookup"><span data-stu-id="c3866-189">Relationships</span></span>
| <span data-ttu-id="c3866-190">关系</span><span class="sxs-lookup"><span data-stu-id="c3866-190">Relationship</span></span> | <span data-ttu-id="c3866-191">类型</span><span class="sxs-lookup"><span data-stu-id="c3866-191">Type</span></span>        | <span data-ttu-id="c3866-192">说明</span><span class="sxs-lookup"><span data-stu-id="c3866-192">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c3866-193">jobs</span><span class="sxs-lookup"><span data-stu-id="c3866-193">jobs</span></span>|<span data-ttu-id="c3866-194">[printJob](printjob.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c3866-194">[printJob](printjob.md) collection</span></span>| <span data-ttu-id="c3866-195">打印机排队等待打印的作业的列表。</span><span class="sxs-lookup"><span data-stu-id="c3866-195">The list of jobs that are queued for printing by the printer.</span></span>|
|<span data-ttu-id="c3866-196">shares</span><span class="sxs-lookup"><span data-stu-id="c3866-196">shares</span></span>|<span data-ttu-id="c3866-197">[printerShare](printershare.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c3866-197">[printerShare](printershare.md) collection</span></span>| <span data-ttu-id="c3866-198">与打印机关联的 printerShares 的列表。</span><span class="sxs-lookup"><span data-stu-id="c3866-198">The list of printerShares that are associated with the printer.</span></span> <span data-ttu-id="c3866-199">目前，只有一个 printerShare 可以与打印机关联。</span><span class="sxs-lookup"><span data-stu-id="c3866-199">Currently, only one printerShare can be associated with the printer.</span></span> <span data-ttu-id="c3866-200">只读。</span><span class="sxs-lookup"><span data-stu-id="c3866-200">Read-only.</span></span> <span data-ttu-id="c3866-201">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="c3866-201">Nullable.</span></span>|
|<span data-ttu-id="c3866-202">插槽</span><span class="sxs-lookup"><span data-stu-id="c3866-202">connectors</span></span>|[<span data-ttu-id="c3866-203">printConnector</span><span class="sxs-lookup"><span data-stu-id="c3866-203">printConnector</span></span>](printconnector.md)|<span data-ttu-id="c3866-204">与打印机关联的连接器。</span><span class="sxs-lookup"><span data-stu-id="c3866-204">The connectors that are associated with the printer.</span></span>|
|<span data-ttu-id="c3866-205">taskTriggers</span><span class="sxs-lookup"><span data-stu-id="c3866-205">taskTriggers</span></span>|<span data-ttu-id="c3866-206">[printTaskTrigger](printtasktrigger.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c3866-206">[printTaskTrigger](printtasktrigger.md) collection</span></span>|<span data-ttu-id="c3866-207">与打印机关联的任务触发器的列表。</span><span class="sxs-lookup"><span data-stu-id="c3866-207">A list of task triggers that are associated with the printer.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c3866-208">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c3866-208">JSON representation</span></span>

<span data-ttu-id="c3866-209">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3866-209">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printer",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "manufacturer": "String",
  "model": "String",
  "isShared": true,
  "registeredDateTime": "String (timestamp)",
  "isAcceptingJobs": true,
  "location": {"@odata.type": "microsoft.graph.printerLocation"},
  "status": {"@odata.type": "microsoft.graph.printerStatus"},
  "defaults": {"@odata.type": "microsoft.graph.printerDefaults"},
  "capabilities": {"@odata.type": "microsoft.graph.printerCapabilities"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


