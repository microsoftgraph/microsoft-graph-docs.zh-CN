---
title: 打印机资源类型
description: 表示已向通用打印服务注册的物理打印机设备。 打印机资源可用于管理打印作业、打印机设置、打印机元数据和注册状态。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 5833dc1f37620a419153100ebf9ce6d7f141fa5d
ms.sourcegitcommit: d9c167f6be71bdb4a023c5ace2733b9854c846d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617008"
---
# <a name="printer-resource-type"></a><span data-ttu-id="0b36f-104">打印机资源类型</span><span class="sxs-lookup"><span data-stu-id="0b36f-104">printer resource type</span></span>

<span data-ttu-id="0b36f-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b36f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b36f-106">表示已向通用打印服务注册的打印机设备。</span><span class="sxs-lookup"><span data-stu-id="0b36f-106">Represents a printer device that has been registered with the Universal Print service.</span></span> <span data-ttu-id="0b36f-107">打印机资源可用于管理打印作业、打印机设置、打印机元数据和注册状态。</span><span class="sxs-lookup"><span data-stu-id="0b36f-107">Printer resources can be used to manage print jobs, printer settings, printer metadata and registration status.</span></span>

## <a name="methods"></a><span data-ttu-id="0b36f-108">方法</span><span class="sxs-lookup"><span data-stu-id="0b36f-108">Methods</span></span>

| <span data-ttu-id="0b36f-109">方法</span><span class="sxs-lookup"><span data-stu-id="0b36f-109">Method</span></span>       | <span data-ttu-id="0b36f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="0b36f-110">Return Type</span></span> | <span data-ttu-id="0b36f-111">说明</span><span class="sxs-lookup"><span data-stu-id="0b36f-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0b36f-112">创建</span><span class="sxs-lookup"><span data-stu-id="0b36f-112">Create</span></span>](../api/printer-create.md) | [<span data-ttu-id="0b36f-113">printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="0b36f-113">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="0b36f-114">创建 (注册) 具有通用打印的新打印机。</span><span class="sxs-lookup"><span data-stu-id="0b36f-114">Create (register) a new printer with Universal Print.</span></span> |
| [<span data-ttu-id="0b36f-115">获取</span><span class="sxs-lookup"><span data-stu-id="0b36f-115">Get</span></span>](../api/printer-get.md) | [<span data-ttu-id="0b36f-116">印刷</span><span class="sxs-lookup"><span data-stu-id="0b36f-116">printer</span></span>](printer.md) | <span data-ttu-id="0b36f-117">读取 printer 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0b36f-117">Read the properties and relationships of the printer object.</span></span> |
| [<span data-ttu-id="0b36f-118">更新</span><span class="sxs-lookup"><span data-stu-id="0b36f-118">Update</span></span>](../api/printer-update.md) | [<span data-ttu-id="0b36f-119">印刷</span><span class="sxs-lookup"><span data-stu-id="0b36f-119">printer</span></span>](printer.md) | <span data-ttu-id="0b36f-120">更新 printer 对象。</span><span class="sxs-lookup"><span data-stu-id="0b36f-120">Update the printer object.</span></span> |
| [<span data-ttu-id="0b36f-121">删除</span><span class="sxs-lookup"><span data-stu-id="0b36f-121">Delete</span></span>](../api/printer-delete.md) | <span data-ttu-id="0b36f-122">无</span><span class="sxs-lookup"><span data-stu-id="0b36f-122">None</span></span> | <span data-ttu-id="0b36f-123">从通用打印服务注销物理打印机。</span><span class="sxs-lookup"><span data-stu-id="0b36f-123">Unregister the physical printer from the Universal Print service.</span></span> |
| [<span data-ttu-id="0b36f-124">restoreFactoryDefaults</span><span class="sxs-lookup"><span data-stu-id="0b36f-124">restoreFactoryDefaults</span></span>](../api/printer-restorefactorydefaults.md) | <span data-ttu-id="0b36f-125">无</span><span class="sxs-lookup"><span data-stu-id="0b36f-125">None</span></span> | <span data-ttu-id="0b36f-126">将打印机的默认设置还原为制造商指定的值。</span><span class="sxs-lookup"><span data-stu-id="0b36f-126">Restore a printer's default settings to the values specified by the manufacturer.</span></span> |
| [<span data-ttu-id="0b36f-127">列出作业</span><span class="sxs-lookup"><span data-stu-id="0b36f-127">List jobs</span></span>](../api/printer-list-jobs.md) | <span data-ttu-id="0b36f-128">[printJob](printjob.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0b36f-128">[printJob](printjob.md) collection</span></span> | <span data-ttu-id="0b36f-129">获取排队等待打印机处理的打印作业的列表。</span><span class="sxs-lookup"><span data-stu-id="0b36f-129">Get a list of print jobs that are queued for processing by the printer.</span></span> |
| [<span data-ttu-id="0b36f-130">创建作业</span><span class="sxs-lookup"><span data-stu-id="0b36f-130">Create job</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="0b36f-131">printJob</span><span class="sxs-lookup"><span data-stu-id="0b36f-131">printJob</span></span>](printjob.md) | <span data-ttu-id="0b36f-132">为打印机创建一个新的打印作业。</span><span class="sxs-lookup"><span data-stu-id="0b36f-132">Create a new print job for the printer.</span></span> <span data-ttu-id="0b36f-133">若要开始打印作业，请使用 [start](../api/printjob-start.md)。</span><span class="sxs-lookup"><span data-stu-id="0b36f-133">To start printing the job, use [start](../api/printjob-start.md).</span></span> |
| [<span data-ttu-id="0b36f-134">List connectors</span><span class="sxs-lookup"><span data-stu-id="0b36f-134">List connectors</span></span>](../api/printer-list-connectors.md) | <span data-ttu-id="0b36f-135">[printConnector](printconnector.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0b36f-135">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="0b36f-136">获取此打印机关联的连接器的列表。</span><span class="sxs-lookup"><span data-stu-id="0b36f-136">Get a list of connectors that this printer is associated with.</span></span> |
| [<span data-ttu-id="0b36f-137">List taskTriggers</span><span class="sxs-lookup"><span data-stu-id="0b36f-137">List taskTriggers</span></span>](../api/printer-list-tasktriggers.md) | <span data-ttu-id="0b36f-138">无</span><span class="sxs-lookup"><span data-stu-id="0b36f-138">None</span></span> | <span data-ttu-id="0b36f-139">列出与此打印机关联的 [printTaskTriggers](printtasktrigger.md) 。</span><span class="sxs-lookup"><span data-stu-id="0b36f-139">List [printTaskTriggers](printtasktrigger.md) associated with this printer.</span></span> |
| [<span data-ttu-id="0b36f-140">Create taskTrigger</span><span class="sxs-lookup"><span data-stu-id="0b36f-140">Create taskTrigger</span></span>](../api/printer-post-tasktriggers.md) | [<span data-ttu-id="0b36f-141">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="0b36f-141">printTaskTrigger</span></span>](printtasktrigger.md) | <span data-ttu-id="0b36f-142">创建在打印事件发生时运行的 [printTaskTrigger](printtasktrigger.md) 。</span><span class="sxs-lookup"><span data-stu-id="0b36f-142">Create a [printTaskTrigger](printtasktrigger.md) that runs when print events occur.</span></span> |
| [<span data-ttu-id="0b36f-143">Delete taskTrigger</span><span class="sxs-lookup"><span data-stu-id="0b36f-143">Delete taskTrigger</span></span>](../api/printer-delete-tasktrigger.md) | <span data-ttu-id="0b36f-144">无</span><span class="sxs-lookup"><span data-stu-id="0b36f-144">None</span></span> | <span data-ttu-id="0b36f-145">删除与打印机关联的 [printTaskTrigger](printtasktrigger.md) 。</span><span class="sxs-lookup"><span data-stu-id="0b36f-145">Delete a [printTaskTrigger](printtasktrigger.md) that is associated with the printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="0b36f-146">属性</span><span class="sxs-lookup"><span data-stu-id="0b36f-146">Properties</span></span>
| <span data-ttu-id="0b36f-147">属性</span><span class="sxs-lookup"><span data-stu-id="0b36f-147">Property</span></span>     | <span data-ttu-id="0b36f-148">类型</span><span class="sxs-lookup"><span data-stu-id="0b36f-148">Type</span></span>        | <span data-ttu-id="0b36f-149">说明</span><span class="sxs-lookup"><span data-stu-id="0b36f-149">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0b36f-150">id</span><span class="sxs-lookup"><span data-stu-id="0b36f-150">id</span></span>|<span data-ttu-id="0b36f-151">String</span><span class="sxs-lookup"><span data-stu-id="0b36f-151">String</span></span>|<span data-ttu-id="0b36f-152">文档的标识符。</span><span class="sxs-lookup"><span data-stu-id="0b36f-152">The document's identifier.</span></span> <span data-ttu-id="0b36f-153">只读。</span><span class="sxs-lookup"><span data-stu-id="0b36f-153">Read-only.</span></span>|
|<span data-ttu-id="0b36f-154">displayName</span><span class="sxs-lookup"><span data-stu-id="0b36f-154">displayName</span></span>|<span data-ttu-id="0b36f-155">String</span><span class="sxs-lookup"><span data-stu-id="0b36f-155">String</span></span>|<span data-ttu-id="0b36f-156">打印机的名称。</span><span class="sxs-lookup"><span data-stu-id="0b36f-156">The name of the printer.</span></span>|
|<span data-ttu-id="0b36f-157">manufacturer</span><span class="sxs-lookup"><span data-stu-id="0b36f-157">manufacturer</span></span>|<span data-ttu-id="0b36f-158">String</span><span class="sxs-lookup"><span data-stu-id="0b36f-158">String</span></span>|<span data-ttu-id="0b36f-159">打印机报告的制造商。</span><span class="sxs-lookup"><span data-stu-id="0b36f-159">The manufacturer reported by the printer.</span></span>|
|<span data-ttu-id="0b36f-160">model</span><span class="sxs-lookup"><span data-stu-id="0b36f-160">model</span></span>|<span data-ttu-id="0b36f-161">String</span><span class="sxs-lookup"><span data-stu-id="0b36f-161">String</span></span>|<span data-ttu-id="0b36f-162">打印机报告的模型名称。</span><span class="sxs-lookup"><span data-stu-id="0b36f-162">The model name reported by the printer.</span></span>|
|<span data-ttu-id="0b36f-163">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="0b36f-163">registeredDateTime</span></span>|<span data-ttu-id="0b36f-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b36f-164">DateTimeOffset</span></span>|<span data-ttu-id="0b36f-165">注册打印机时的 DateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="0b36f-165">The DateTimeOffset when the printer was registered.</span></span> <span data-ttu-id="0b36f-166">只读。</span><span class="sxs-lookup"><span data-stu-id="0b36f-166">Read-only.</span></span>|
|<span data-ttu-id="0b36f-167">status</span><span class="sxs-lookup"><span data-stu-id="0b36f-167">status</span></span>|[<span data-ttu-id="0b36f-168">printerStatus</span><span class="sxs-lookup"><span data-stu-id="0b36f-168">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="0b36f-169">打印机的处理状态，包括任何错误。</span><span class="sxs-lookup"><span data-stu-id="0b36f-169">The processing status of the printer, including any errors.</span></span>|
|<span data-ttu-id="0b36f-170">isShared</span><span class="sxs-lookup"><span data-stu-id="0b36f-170">isShared</span></span>|<span data-ttu-id="0b36f-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b36f-171">Boolean</span></span>|<span data-ttu-id="0b36f-172">如果打印机是共享的，则为 True;否则为 false。</span><span class="sxs-lookup"><span data-stu-id="0b36f-172">True if the printer is shared; false otherwise.</span></span> <span data-ttu-id="0b36f-173">只读。</span><span class="sxs-lookup"><span data-stu-id="0b36f-173">Read-only.</span></span>|
|<span data-ttu-id="0b36f-174">hasPhysicalDevice</span><span class="sxs-lookup"><span data-stu-id="0b36f-174">hasPhysicalDevice</span></span>|<span data-ttu-id="0b36f-175">布尔值</span><span class="sxs-lookup"><span data-stu-id="0b36f-175">Boolean</span></span>|<span data-ttu-id="0b36f-176">如此如果打印机有物理设备进行打印。</span><span class="sxs-lookup"><span data-stu-id="0b36f-176">True if the printer has a physical device for printing.</span></span> <span data-ttu-id="0b36f-177">只读。</span><span class="sxs-lookup"><span data-stu-id="0b36f-177">Read-only.</span></span>|
|<span data-ttu-id="0b36f-178">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="0b36f-178">isAcceptingJobs</span></span>|<span data-ttu-id="0b36f-179">布尔值</span><span class="sxs-lookup"><span data-stu-id="0b36f-179">Boolean</span></span>|<span data-ttu-id="0b36f-180">打印机当前是否正在接受新的打印作业。</span><span class="sxs-lookup"><span data-stu-id="0b36f-180">Whether the printer is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="0b36f-181">位置</span><span class="sxs-lookup"><span data-stu-id="0b36f-181">location</span></span>|[<span data-ttu-id="0b36f-182">printerLocation</span><span class="sxs-lookup"><span data-stu-id="0b36f-182">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="0b36f-183">打印机的物理和/或组织位置。</span><span class="sxs-lookup"><span data-stu-id="0b36f-183">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="0b36f-184">defaults</span><span class="sxs-lookup"><span data-stu-id="0b36f-184">defaults</span></span>|[<span data-ttu-id="0b36f-185">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="0b36f-185">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="0b36f-186">打印机的默认打印设置。</span><span class="sxs-lookup"><span data-stu-id="0b36f-186">The printer's default print settings.</span></span>|
|<span data-ttu-id="0b36f-187">capabilities</span><span class="sxs-lookup"><span data-stu-id="0b36f-187">capabilities</span></span>|[<span data-ttu-id="0b36f-188">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="0b36f-188">printerCapabilities</span></span>](printercapabilities.md)|<span data-ttu-id="0b36f-189">与此打印机共享相关联的打印机的功能。</span><span class="sxs-lookup"><span data-stu-id="0b36f-189">The capabilities of the printer associated with this printer share.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b36f-190">关系</span><span class="sxs-lookup"><span data-stu-id="0b36f-190">Relationships</span></span>
| <span data-ttu-id="0b36f-191">关系</span><span class="sxs-lookup"><span data-stu-id="0b36f-191">Relationship</span></span> | <span data-ttu-id="0b36f-192">类型</span><span class="sxs-lookup"><span data-stu-id="0b36f-192">Type</span></span>        | <span data-ttu-id="0b36f-193">说明</span><span class="sxs-lookup"><span data-stu-id="0b36f-193">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0b36f-194">jobs</span><span class="sxs-lookup"><span data-stu-id="0b36f-194">jobs</span></span>|<span data-ttu-id="0b36f-195">[printJob](printjob.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0b36f-195">[printJob](printjob.md) collection</span></span>| <span data-ttu-id="0b36f-196">打印机排队等待打印的作业的列表。</span><span class="sxs-lookup"><span data-stu-id="0b36f-196">The list of jobs that are queued for printing by the printer.</span></span>|
|<span data-ttu-id="0b36f-197">shares</span><span class="sxs-lookup"><span data-stu-id="0b36f-197">shares</span></span>|<span data-ttu-id="0b36f-198">[printerShare](printershare.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0b36f-198">[printerShare](printershare.md) collection</span></span>| <span data-ttu-id="0b36f-199">与打印机关联的 printerShares 的列表。</span><span class="sxs-lookup"><span data-stu-id="0b36f-199">The list of printerShares that are associated with the printer.</span></span> <span data-ttu-id="0b36f-200">目前，只有一个 printerShare 可以与打印机关联。</span><span class="sxs-lookup"><span data-stu-id="0b36f-200">Currently, only one printerShare can be associated with the printer.</span></span> <span data-ttu-id="0b36f-201">只读。</span><span class="sxs-lookup"><span data-stu-id="0b36f-201">Read-only.</span></span> <span data-ttu-id="0b36f-202">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="0b36f-202">Nullable.</span></span>|
|<span data-ttu-id="0b36f-203">插槽</span><span class="sxs-lookup"><span data-stu-id="0b36f-203">connectors</span></span>|[<span data-ttu-id="0b36f-204">printConnector</span><span class="sxs-lookup"><span data-stu-id="0b36f-204">printConnector</span></span>](printconnector.md)|<span data-ttu-id="0b36f-205">与打印机关联的连接器。</span><span class="sxs-lookup"><span data-stu-id="0b36f-205">The connectors that are associated with the printer.</span></span>|
|<span data-ttu-id="0b36f-206">taskTriggers</span><span class="sxs-lookup"><span data-stu-id="0b36f-206">taskTriggers</span></span>|<span data-ttu-id="0b36f-207">[printTaskTrigger](printtasktrigger.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0b36f-207">[printTaskTrigger](printtasktrigger.md) collection</span></span>|<span data-ttu-id="0b36f-208">与打印机关联的任务触发器的列表。</span><span class="sxs-lookup"><span data-stu-id="0b36f-208">A list of task triggers that are associated with the printer.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0b36f-209">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0b36f-209">JSON representation</span></span>

<span data-ttu-id="0b36f-210">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b36f-210">The following is a JSON representation of the resource.</span></span>

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
  "hasPhysicalDevice": true,
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


