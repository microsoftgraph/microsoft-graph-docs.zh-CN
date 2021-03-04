---
title: 打印机资源类型
description: 表示已在通用打印服务中注册的物理打印机设备。 打印机资源可用于管理打印作业、打印机设置、打印机元数据和注册状态。
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 9adb08cd553857cbc7f7f9ebb257773b8775fa3f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442885"
---
# <a name="printer-resource-type"></a><span data-ttu-id="cc325-104">打印机资源类型</span><span class="sxs-lookup"><span data-stu-id="cc325-104">printer resource type</span></span>

<span data-ttu-id="cc325-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc325-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc325-106">表示已在通用打印服务中注册的打印机设备。</span><span class="sxs-lookup"><span data-stu-id="cc325-106">Represents a printer device that has been registered with the Universal Print service.</span></span> <span data-ttu-id="cc325-107">打印机资源可用于管理打印作业、打印机设置、打印机元数据和注册状态。</span><span class="sxs-lookup"><span data-stu-id="cc325-107">Printer resources can be used to manage print jobs, printer settings, printer metadata and registration status.</span></span>

<span data-ttu-id="cc325-108">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="cc325-108">This resource supports:</span></span>
* <span data-ttu-id="cc325-109">[订阅更改通知](/graph/universal-print-webhook-notifications)。</span><span class="sxs-lookup"><span data-stu-id="cc325-109">[Subscribing to change notifications](/graph/universal-print-webhook-notifications).</span></span>

## <a name="methods"></a><span data-ttu-id="cc325-110">Methods</span><span class="sxs-lookup"><span data-stu-id="cc325-110">Methods</span></span>

| <span data-ttu-id="cc325-111">方法</span><span class="sxs-lookup"><span data-stu-id="cc325-111">Method</span></span>       | <span data-ttu-id="cc325-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="cc325-112">Return Type</span></span> | <span data-ttu-id="cc325-113">说明</span><span class="sxs-lookup"><span data-stu-id="cc325-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="cc325-114">创建</span><span class="sxs-lookup"><span data-stu-id="cc325-114">Create</span></span>](../api/printer-create.md) | [<span data-ttu-id="cc325-115">printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="cc325-115">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="cc325-116">创建 (通用) 新打印机上注册。</span><span class="sxs-lookup"><span data-stu-id="cc325-116">Create (register) a new printer with Universal Print.</span></span> |
| [<span data-ttu-id="cc325-117">获取</span><span class="sxs-lookup"><span data-stu-id="cc325-117">Get</span></span>](../api/printer-get.md) | [<span data-ttu-id="cc325-118">打印机</span><span class="sxs-lookup"><span data-stu-id="cc325-118">printer</span></span>](printer.md) | <span data-ttu-id="cc325-119">读取打印机对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cc325-119">Read the properties and relationships of the printer object.</span></span> |
| [<span data-ttu-id="cc325-120">更新</span><span class="sxs-lookup"><span data-stu-id="cc325-120">Update</span></span>](../api/printer-update.md) | [<span data-ttu-id="cc325-121">打印机</span><span class="sxs-lookup"><span data-stu-id="cc325-121">printer</span></span>](printer.md) | <span data-ttu-id="cc325-122">更新打印机对象。</span><span class="sxs-lookup"><span data-stu-id="cc325-122">Update the printer object.</span></span> |
| [<span data-ttu-id="cc325-123">删除</span><span class="sxs-lookup"><span data-stu-id="cc325-123">Delete</span></span>](../api/printer-delete.md) | <span data-ttu-id="cc325-124">无</span><span class="sxs-lookup"><span data-stu-id="cc325-124">None</span></span> | <span data-ttu-id="cc325-125">从通用打印服务中注销物理打印机。</span><span class="sxs-lookup"><span data-stu-id="cc325-125">Unregister the physical printer from the Universal Print service.</span></span> |
| [<span data-ttu-id="cc325-126">restoreFactoryDefaults</span><span class="sxs-lookup"><span data-stu-id="cc325-126">restoreFactoryDefaults</span></span>](../api/printer-restorefactorydefaults.md) | <span data-ttu-id="cc325-127">无</span><span class="sxs-lookup"><span data-stu-id="cc325-127">None</span></span> | <span data-ttu-id="cc325-128">将打印机的默认设置还原到制造商指定的值。</span><span class="sxs-lookup"><span data-stu-id="cc325-128">Restore a printer's default settings to the values specified by the manufacturer.</span></span> |
| [<span data-ttu-id="cc325-129">列出作业</span><span class="sxs-lookup"><span data-stu-id="cc325-129">List jobs</span></span>](../api/printer-list-jobs.md) | <span data-ttu-id="cc325-130">[printJob](printjob.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cc325-130">[printJob](printjob.md) collection</span></span> | <span data-ttu-id="cc325-131">获取已排入队列以由打印机处理的打印作业的列表。</span><span class="sxs-lookup"><span data-stu-id="cc325-131">Get a list of print jobs that are queued for processing by the printer.</span></span> |
| [<span data-ttu-id="cc325-132">创建作业</span><span class="sxs-lookup"><span data-stu-id="cc325-132">Create job</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="cc325-133">printJob</span><span class="sxs-lookup"><span data-stu-id="cc325-133">printJob</span></span>](printjob.md) | <span data-ttu-id="cc325-134">为打印机创建新的打印作业。</span><span class="sxs-lookup"><span data-stu-id="cc325-134">Create a new print job for the printer.</span></span> <span data-ttu-id="cc325-135">若要开始打印作业，请使用"开始["。](../api/printjob-start.md)</span><span class="sxs-lookup"><span data-stu-id="cc325-135">To start printing the job, use [start](../api/printjob-start.md).</span></span> |
| [<span data-ttu-id="cc325-136">List connectors</span><span class="sxs-lookup"><span data-stu-id="cc325-136">List connectors</span></span>](../api/printer-list-connectors.md) | <span data-ttu-id="cc325-137">[printConnector](printconnector.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cc325-137">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="cc325-138">获取与此打印机关联的连接器列表。</span><span class="sxs-lookup"><span data-stu-id="cc325-138">Get a list of connectors that this printer is associated with.</span></span> |
| [<span data-ttu-id="cc325-139">List taskTriggers</span><span class="sxs-lookup"><span data-stu-id="cc325-139">List taskTriggers</span></span>](../api/printer-list-tasktriggers.md) | <span data-ttu-id="cc325-140">无</span><span class="sxs-lookup"><span data-stu-id="cc325-140">None</span></span> | <span data-ttu-id="cc325-141">列出[与此打印机关联的 printTaskTriggers。](printtasktrigger.md)</span><span class="sxs-lookup"><span data-stu-id="cc325-141">List [printTaskTriggers](printtasktrigger.md) associated with this printer.</span></span> |
| [<span data-ttu-id="cc325-142">Create taskTrigger</span><span class="sxs-lookup"><span data-stu-id="cc325-142">Create taskTrigger</span></span>](../api/printer-post-tasktriggers.md) | [<span data-ttu-id="cc325-143">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="cc325-143">printTaskTrigger</span></span>](printtasktrigger.md) | <span data-ttu-id="cc325-144">创建在打印事件发生时运行的[printTaskTrigger。](printtasktrigger.md)</span><span class="sxs-lookup"><span data-stu-id="cc325-144">Create a [printTaskTrigger](printtasktrigger.md) that runs when print events occur.</span></span> |
| [<span data-ttu-id="cc325-145">Delete taskTrigger</span><span class="sxs-lookup"><span data-stu-id="cc325-145">Delete taskTrigger</span></span>](../api/printer-delete-tasktrigger.md) | <span data-ttu-id="cc325-146">无</span><span class="sxs-lookup"><span data-stu-id="cc325-146">None</span></span> | <span data-ttu-id="cc325-147">删除[与打印机关联的 printTaskTrigger。](printtasktrigger.md)</span><span class="sxs-lookup"><span data-stu-id="cc325-147">Delete a [printTaskTrigger](printtasktrigger.md) that is associated with the printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="cc325-148">属性</span><span class="sxs-lookup"><span data-stu-id="cc325-148">Properties</span></span>
| <span data-ttu-id="cc325-149">属性</span><span class="sxs-lookup"><span data-stu-id="cc325-149">Property</span></span>     | <span data-ttu-id="cc325-150">类型</span><span class="sxs-lookup"><span data-stu-id="cc325-150">Type</span></span>        | <span data-ttu-id="cc325-151">说明</span><span class="sxs-lookup"><span data-stu-id="cc325-151">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cc325-152">id</span><span class="sxs-lookup"><span data-stu-id="cc325-152">id</span></span>|<span data-ttu-id="cc325-153">String</span><span class="sxs-lookup"><span data-stu-id="cc325-153">String</span></span>|<span data-ttu-id="cc325-154">文档的标识符。</span><span class="sxs-lookup"><span data-stu-id="cc325-154">The document's identifier.</span></span> <span data-ttu-id="cc325-155">只读。</span><span class="sxs-lookup"><span data-stu-id="cc325-155">Read-only.</span></span>|
|<span data-ttu-id="cc325-156">displayName</span><span class="sxs-lookup"><span data-stu-id="cc325-156">displayName</span></span>|<span data-ttu-id="cc325-157">String</span><span class="sxs-lookup"><span data-stu-id="cc325-157">String</span></span>|<span data-ttu-id="cc325-158">打印机的名称。</span><span class="sxs-lookup"><span data-stu-id="cc325-158">The name of the printer.</span></span>|
|<span data-ttu-id="cc325-159">manufacturer</span><span class="sxs-lookup"><span data-stu-id="cc325-159">manufacturer</span></span>|<span data-ttu-id="cc325-160">String</span><span class="sxs-lookup"><span data-stu-id="cc325-160">String</span></span>|<span data-ttu-id="cc325-161">打印机报告的制造商。</span><span class="sxs-lookup"><span data-stu-id="cc325-161">The manufacturer reported by the printer.</span></span>|
|<span data-ttu-id="cc325-162">model</span><span class="sxs-lookup"><span data-stu-id="cc325-162">model</span></span>|<span data-ttu-id="cc325-163">String</span><span class="sxs-lookup"><span data-stu-id="cc325-163">String</span></span>|<span data-ttu-id="cc325-164">打印机报告的型号名称。</span><span class="sxs-lookup"><span data-stu-id="cc325-164">The model name reported by the printer.</span></span>|
|<span data-ttu-id="cc325-165">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="cc325-165">registeredDateTime</span></span>|<span data-ttu-id="cc325-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc325-166">DateTimeOffset</span></span>|<span data-ttu-id="cc325-167">注册打印机时的日期时间Offset。</span><span class="sxs-lookup"><span data-stu-id="cc325-167">The DateTimeOffset when the printer was registered.</span></span> <span data-ttu-id="cc325-168">只读。</span><span class="sxs-lookup"><span data-stu-id="cc325-168">Read-only.</span></span>|
|<span data-ttu-id="cc325-169">status</span><span class="sxs-lookup"><span data-stu-id="cc325-169">status</span></span>|[<span data-ttu-id="cc325-170">printerStatus</span><span class="sxs-lookup"><span data-stu-id="cc325-170">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="cc325-171">打印机的处理状态，包括任何错误。</span><span class="sxs-lookup"><span data-stu-id="cc325-171">The processing status of the printer, including any errors.</span></span>|
|<span data-ttu-id="cc325-172">isShared</span><span class="sxs-lookup"><span data-stu-id="cc325-172">isShared</span></span>|<span data-ttu-id="cc325-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc325-173">Boolean</span></span>|<span data-ttu-id="cc325-174">如果共享打印机，则其为 True;否则为 false。</span><span class="sxs-lookup"><span data-stu-id="cc325-174">True if the printer is shared; false otherwise.</span></span> <span data-ttu-id="cc325-175">只读。</span><span class="sxs-lookup"><span data-stu-id="cc325-175">Read-only.</span></span>|
|<span data-ttu-id="cc325-176">hasPhysicalDevice</span><span class="sxs-lookup"><span data-stu-id="cc325-176">hasPhysicalDevice</span></span>|<span data-ttu-id="cc325-177">布尔</span><span class="sxs-lookup"><span data-stu-id="cc325-177">Boolean</span></span>|<span data-ttu-id="cc325-178">如此 如果打印机具有用于打印的物理设备。</span><span class="sxs-lookup"><span data-stu-id="cc325-178">True if the printer has a physical device for printing.</span></span> <span data-ttu-id="cc325-179">只读。</span><span class="sxs-lookup"><span data-stu-id="cc325-179">Read-only.</span></span>|
|<span data-ttu-id="cc325-180">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="cc325-180">isAcceptingJobs</span></span>|<span data-ttu-id="cc325-181">布尔</span><span class="sxs-lookup"><span data-stu-id="cc325-181">Boolean</span></span>|<span data-ttu-id="cc325-182">打印机当前是否接受新的打印作业。</span><span class="sxs-lookup"><span data-stu-id="cc325-182">Whether the printer is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="cc325-183">位置</span><span class="sxs-lookup"><span data-stu-id="cc325-183">location</span></span>|[<span data-ttu-id="cc325-184">printerLocation</span><span class="sxs-lookup"><span data-stu-id="cc325-184">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="cc325-185">打印机的物理和/或组织位置。</span><span class="sxs-lookup"><span data-stu-id="cc325-185">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="cc325-186">defaults</span><span class="sxs-lookup"><span data-stu-id="cc325-186">defaults</span></span>|[<span data-ttu-id="cc325-187">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="cc325-187">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="cc325-188">打印机的默认打印设置。</span><span class="sxs-lookup"><span data-stu-id="cc325-188">The printer's default print settings.</span></span>|
|<span data-ttu-id="cc325-189">capabilities</span><span class="sxs-lookup"><span data-stu-id="cc325-189">capabilities</span></span>|[<span data-ttu-id="cc325-190">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="cc325-190">printerCapabilities</span></span>](printercapabilities.md)|<span data-ttu-id="cc325-191">与此打印机共享关联的打印机的功能。</span><span class="sxs-lookup"><span data-stu-id="cc325-191">The capabilities of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="cc325-192">lastSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="cc325-192">lastSeenDateTime</span></span>|<span data-ttu-id="cc325-193">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc325-193">DateTimeOffset</span></span>|<span data-ttu-id="cc325-194">打印机与通用打印交互时的最新 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="cc325-194">The most recent dateTimeOffset when a printer interacted with Universal Print.</span></span> <span data-ttu-id="cc325-195">只读。</span><span class="sxs-lookup"><span data-stu-id="cc325-195">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc325-196">关系</span><span class="sxs-lookup"><span data-stu-id="cc325-196">Relationships</span></span>
| <span data-ttu-id="cc325-197">关系</span><span class="sxs-lookup"><span data-stu-id="cc325-197">Relationship</span></span> | <span data-ttu-id="cc325-198">类型</span><span class="sxs-lookup"><span data-stu-id="cc325-198">Type</span></span>        | <span data-ttu-id="cc325-199">说明</span><span class="sxs-lookup"><span data-stu-id="cc325-199">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cc325-200">jobs</span><span class="sxs-lookup"><span data-stu-id="cc325-200">jobs</span></span>|<span data-ttu-id="cc325-201">[printJob](printjob.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cc325-201">[printJob](printjob.md) collection</span></span>| <span data-ttu-id="cc325-202">由打印机排入打印队列的作业列表。</span><span class="sxs-lookup"><span data-stu-id="cc325-202">The list of jobs that are queued for printing by the printer.</span></span>|
|<span data-ttu-id="cc325-203">shares</span><span class="sxs-lookup"><span data-stu-id="cc325-203">shares</span></span>|<span data-ttu-id="cc325-204">[printerShare](printershare.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cc325-204">[printerShare](printershare.md) collection</span></span>| <span data-ttu-id="cc325-205">与打印机关联的 printerShares 列表。</span><span class="sxs-lookup"><span data-stu-id="cc325-205">The list of printerShares that are associated with the printer.</span></span> <span data-ttu-id="cc325-206">目前，只能将一个 printerShare 与打印机关联。</span><span class="sxs-lookup"><span data-stu-id="cc325-206">Currently, only one printerShare can be associated with the printer.</span></span> <span data-ttu-id="cc325-207">只读。</span><span class="sxs-lookup"><span data-stu-id="cc325-207">Read-only.</span></span> <span data-ttu-id="cc325-208">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="cc325-208">Nullable.</span></span>|
|<span data-ttu-id="cc325-209">连接器</span><span class="sxs-lookup"><span data-stu-id="cc325-209">connectors</span></span>|[<span data-ttu-id="cc325-210">printConnector</span><span class="sxs-lookup"><span data-stu-id="cc325-210">printConnector</span></span>](printconnector.md)|<span data-ttu-id="cc325-211">与打印机关联的连接器。</span><span class="sxs-lookup"><span data-stu-id="cc325-211">The connectors that are associated with the printer.</span></span>|
|<span data-ttu-id="cc325-212">taskTriggers</span><span class="sxs-lookup"><span data-stu-id="cc325-212">taskTriggers</span></span>|<span data-ttu-id="cc325-213">[printTaskTrigger](printtasktrigger.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cc325-213">[printTaskTrigger](printtasktrigger.md) collection</span></span>|<span data-ttu-id="cc325-214">与打印机关联的任务触发器列表。</span><span class="sxs-lookup"><span data-stu-id="cc325-214">A list of task triggers that are associated with the printer.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cc325-215">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cc325-215">JSON representation</span></span>

<span data-ttu-id="cc325-216">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc325-216">The following is a JSON representation of the resource.</span></span>

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
  "capabilities": {"@odata.type": "microsoft.graph.printerCapabilities"},
  "lastSeenDateTime": "String (timestamp)"
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


