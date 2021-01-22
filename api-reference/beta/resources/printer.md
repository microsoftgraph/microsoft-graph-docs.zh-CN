---
title: 打印机资源类型
description: 表示已在通用打印服务中注册的物理打印机设备。 打印机资源可用于管理打印作业、打印机设置、打印机元数据和注册状态。
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: fab3e933608143846555c556a215025e39666257
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934868"
---
# <a name="printer-resource-type"></a><span data-ttu-id="b8f30-104">打印机资源类型</span><span class="sxs-lookup"><span data-stu-id="b8f30-104">printer resource type</span></span>

<span data-ttu-id="b8f30-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8f30-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8f30-106">表示已在通用打印服务中注册的打印机设备。</span><span class="sxs-lookup"><span data-stu-id="b8f30-106">Represents a printer device that has been registered with the Universal Print service.</span></span> <span data-ttu-id="b8f30-107">打印机资源可用于管理打印作业、打印机设置、打印机元数据和注册状态。</span><span class="sxs-lookup"><span data-stu-id="b8f30-107">Printer resources can be used to manage print jobs, printer settings, printer metadata and registration status.</span></span>

<span data-ttu-id="b8f30-108">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="b8f30-108">This resource supports:</span></span>
* <span data-ttu-id="b8f30-109">[订阅更改通知](/graph/universal-print-webhook-notifications)。</span><span class="sxs-lookup"><span data-stu-id="b8f30-109">[Subscribing to change notifications](/graph/universal-print-webhook-notifications).</span></span>

## <a name="methods"></a><span data-ttu-id="b8f30-110">方法</span><span class="sxs-lookup"><span data-stu-id="b8f30-110">Methods</span></span>

| <span data-ttu-id="b8f30-111">方法</span><span class="sxs-lookup"><span data-stu-id="b8f30-111">Method</span></span>       | <span data-ttu-id="b8f30-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="b8f30-112">Return Type</span></span> | <span data-ttu-id="b8f30-113">说明</span><span class="sxs-lookup"><span data-stu-id="b8f30-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b8f30-114">创建</span><span class="sxs-lookup"><span data-stu-id="b8f30-114">Create</span></span>](../api/printer-create.md) | [<span data-ttu-id="b8f30-115">printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="b8f30-115">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="b8f30-116">创建 (通用) 新打印机进行注册。</span><span class="sxs-lookup"><span data-stu-id="b8f30-116">Create (register) a new printer with Universal Print.</span></span> |
| [<span data-ttu-id="b8f30-117">获取</span><span class="sxs-lookup"><span data-stu-id="b8f30-117">Get</span></span>](../api/printer-get.md) | [<span data-ttu-id="b8f30-118">printer</span><span class="sxs-lookup"><span data-stu-id="b8f30-118">printer</span></span>](printer.md) | <span data-ttu-id="b8f30-119">读取打印机对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b8f30-119">Read the properties and relationships of the printer object.</span></span> |
| [<span data-ttu-id="b8f30-120">更新</span><span class="sxs-lookup"><span data-stu-id="b8f30-120">Update</span></span>](../api/printer-update.md) | [<span data-ttu-id="b8f30-121">printer</span><span class="sxs-lookup"><span data-stu-id="b8f30-121">printer</span></span>](printer.md) | <span data-ttu-id="b8f30-122">更新打印机对象。</span><span class="sxs-lookup"><span data-stu-id="b8f30-122">Update the printer object.</span></span> |
| [<span data-ttu-id="b8f30-123">删除</span><span class="sxs-lookup"><span data-stu-id="b8f30-123">Delete</span></span>](../api/printer-delete.md) | <span data-ttu-id="b8f30-124">无</span><span class="sxs-lookup"><span data-stu-id="b8f30-124">None</span></span> | <span data-ttu-id="b8f30-125">从通用打印服务中注销物理打印机。</span><span class="sxs-lookup"><span data-stu-id="b8f30-125">Unregister the physical printer from the Universal Print service.</span></span> |
| [<span data-ttu-id="b8f30-126">restoreFactoryDefaults</span><span class="sxs-lookup"><span data-stu-id="b8f30-126">restoreFactoryDefaults</span></span>](../api/printer-restorefactorydefaults.md) | <span data-ttu-id="b8f30-127">无</span><span class="sxs-lookup"><span data-stu-id="b8f30-127">None</span></span> | <span data-ttu-id="b8f30-128">将打印机的默认设置还原到制造商指定的值。</span><span class="sxs-lookup"><span data-stu-id="b8f30-128">Restore a printer's default settings to the values specified by the manufacturer.</span></span> |
| [<span data-ttu-id="b8f30-129">列出作业</span><span class="sxs-lookup"><span data-stu-id="b8f30-129">List jobs</span></span>](../api/printer-list-jobs.md) | <span data-ttu-id="b8f30-130">[printJob](printjob.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b8f30-130">[printJob](printjob.md) collection</span></span> | <span data-ttu-id="b8f30-131">获取由打印机排队进行处理的打印作业的列表。</span><span class="sxs-lookup"><span data-stu-id="b8f30-131">Get a list of print jobs that are queued for processing by the printer.</span></span> |
| [<span data-ttu-id="b8f30-132">创建作业</span><span class="sxs-lookup"><span data-stu-id="b8f30-132">Create job</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="b8f30-133">printJob</span><span class="sxs-lookup"><span data-stu-id="b8f30-133">printJob</span></span>](printjob.md) | <span data-ttu-id="b8f30-134">为打印机创建新的打印作业。</span><span class="sxs-lookup"><span data-stu-id="b8f30-134">Create a new print job for the printer.</span></span> <span data-ttu-id="b8f30-135">若要开始打印作业，请使用"开始["。](../api/printjob-start.md)</span><span class="sxs-lookup"><span data-stu-id="b8f30-135">To start printing the job, use [start](../api/printjob-start.md).</span></span> |
| [<span data-ttu-id="b8f30-136">List connectors</span><span class="sxs-lookup"><span data-stu-id="b8f30-136">List connectors</span></span>](../api/printer-list-connectors.md) | <span data-ttu-id="b8f30-137">[printConnector](printconnector.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b8f30-137">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="b8f30-138">获取与此打印机关联的连接器列表。</span><span class="sxs-lookup"><span data-stu-id="b8f30-138">Get a list of connectors that this printer is associated with.</span></span> |
| [<span data-ttu-id="b8f30-139">List taskTriggers</span><span class="sxs-lookup"><span data-stu-id="b8f30-139">List taskTriggers</span></span>](../api/printer-list-tasktriggers.md) | <span data-ttu-id="b8f30-140">无</span><span class="sxs-lookup"><span data-stu-id="b8f30-140">None</span></span> | <span data-ttu-id="b8f30-141">列出[与此打印机关联的 printTaskTriggers。](printtasktrigger.md)</span><span class="sxs-lookup"><span data-stu-id="b8f30-141">List [printTaskTriggers](printtasktrigger.md) associated with this printer.</span></span> |
| [<span data-ttu-id="b8f30-142">Create taskTrigger</span><span class="sxs-lookup"><span data-stu-id="b8f30-142">Create taskTrigger</span></span>](../api/printer-post-tasktriggers.md) | [<span data-ttu-id="b8f30-143">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="b8f30-143">printTaskTrigger</span></span>](printtasktrigger.md) | <span data-ttu-id="b8f30-144">创建在打印事件发生时运行的[printTaskTrigger。](printtasktrigger.md)</span><span class="sxs-lookup"><span data-stu-id="b8f30-144">Create a [printTaskTrigger](printtasktrigger.md) that runs when print events occur.</span></span> |
| [<span data-ttu-id="b8f30-145">Delete taskTrigger</span><span class="sxs-lookup"><span data-stu-id="b8f30-145">Delete taskTrigger</span></span>](../api/printer-delete-tasktrigger.md) | <span data-ttu-id="b8f30-146">无</span><span class="sxs-lookup"><span data-stu-id="b8f30-146">None</span></span> | <span data-ttu-id="b8f30-147">删除[与打印机关联的 printTaskTrigger。](printtasktrigger.md)</span><span class="sxs-lookup"><span data-stu-id="b8f30-147">Delete a [printTaskTrigger](printtasktrigger.md) that is associated with the printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="b8f30-148">属性</span><span class="sxs-lookup"><span data-stu-id="b8f30-148">Properties</span></span>
| <span data-ttu-id="b8f30-149">属性</span><span class="sxs-lookup"><span data-stu-id="b8f30-149">Property</span></span>     | <span data-ttu-id="b8f30-150">类型</span><span class="sxs-lookup"><span data-stu-id="b8f30-150">Type</span></span>        | <span data-ttu-id="b8f30-151">说明</span><span class="sxs-lookup"><span data-stu-id="b8f30-151">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b8f30-152">id</span><span class="sxs-lookup"><span data-stu-id="b8f30-152">id</span></span>|<span data-ttu-id="b8f30-153">String</span><span class="sxs-lookup"><span data-stu-id="b8f30-153">String</span></span>|<span data-ttu-id="b8f30-154">文档的标识符。</span><span class="sxs-lookup"><span data-stu-id="b8f30-154">The document's identifier.</span></span> <span data-ttu-id="b8f30-155">只读。</span><span class="sxs-lookup"><span data-stu-id="b8f30-155">Read-only.</span></span>|
|<span data-ttu-id="b8f30-156">displayName</span><span class="sxs-lookup"><span data-stu-id="b8f30-156">displayName</span></span>|<span data-ttu-id="b8f30-157">String</span><span class="sxs-lookup"><span data-stu-id="b8f30-157">String</span></span>|<span data-ttu-id="b8f30-158">打印机的名称。</span><span class="sxs-lookup"><span data-stu-id="b8f30-158">The name of the printer.</span></span>|
|<span data-ttu-id="b8f30-159">manufacturer</span><span class="sxs-lookup"><span data-stu-id="b8f30-159">manufacturer</span></span>|<span data-ttu-id="b8f30-160">String</span><span class="sxs-lookup"><span data-stu-id="b8f30-160">String</span></span>|<span data-ttu-id="b8f30-161">打印机报告的制造商。</span><span class="sxs-lookup"><span data-stu-id="b8f30-161">The manufacturer reported by the printer.</span></span>|
|<span data-ttu-id="b8f30-162">model</span><span class="sxs-lookup"><span data-stu-id="b8f30-162">model</span></span>|<span data-ttu-id="b8f30-163">String</span><span class="sxs-lookup"><span data-stu-id="b8f30-163">String</span></span>|<span data-ttu-id="b8f30-164">打印机报告的型号名称。</span><span class="sxs-lookup"><span data-stu-id="b8f30-164">The model name reported by the printer.</span></span>|
|<span data-ttu-id="b8f30-165">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="b8f30-165">registeredDateTime</span></span>|<span data-ttu-id="b8f30-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8f30-166">DateTimeOffset</span></span>|<span data-ttu-id="b8f30-167">注册打印机时的日期时间Offset。</span><span class="sxs-lookup"><span data-stu-id="b8f30-167">The DateTimeOffset when the printer was registered.</span></span> <span data-ttu-id="b8f30-168">只读。</span><span class="sxs-lookup"><span data-stu-id="b8f30-168">Read-only.</span></span>|
|<span data-ttu-id="b8f30-169">状态</span><span class="sxs-lookup"><span data-stu-id="b8f30-169">status</span></span>|[<span data-ttu-id="b8f30-170">printerStatus</span><span class="sxs-lookup"><span data-stu-id="b8f30-170">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="b8f30-171">打印机的处理状态，包括任何错误。</span><span class="sxs-lookup"><span data-stu-id="b8f30-171">The processing status of the printer, including any errors.</span></span>|
|<span data-ttu-id="b8f30-172">isShared</span><span class="sxs-lookup"><span data-stu-id="b8f30-172">isShared</span></span>|<span data-ttu-id="b8f30-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8f30-173">Boolean</span></span>|<span data-ttu-id="b8f30-174">如果共享打印机，则其为 True;否则为 false。</span><span class="sxs-lookup"><span data-stu-id="b8f30-174">True if the printer is shared; false otherwise.</span></span> <span data-ttu-id="b8f30-175">只读。</span><span class="sxs-lookup"><span data-stu-id="b8f30-175">Read-only.</span></span>|
|<span data-ttu-id="b8f30-176">hasPhysicalDevice</span><span class="sxs-lookup"><span data-stu-id="b8f30-176">hasPhysicalDevice</span></span>|<span data-ttu-id="b8f30-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8f30-177">Boolean</span></span>|<span data-ttu-id="b8f30-178">如此 如果打印机具有用于打印的物理设备。</span><span class="sxs-lookup"><span data-stu-id="b8f30-178">True if the printer has a physical device for printing.</span></span> <span data-ttu-id="b8f30-179">只读。</span><span class="sxs-lookup"><span data-stu-id="b8f30-179">Read-only.</span></span>|
|<span data-ttu-id="b8f30-180">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="b8f30-180">isAcceptingJobs</span></span>|<span data-ttu-id="b8f30-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8f30-181">Boolean</span></span>|<span data-ttu-id="b8f30-182">打印机当前是否接受新的打印作业。</span><span class="sxs-lookup"><span data-stu-id="b8f30-182">Whether the printer is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="b8f30-183">location</span><span class="sxs-lookup"><span data-stu-id="b8f30-183">location</span></span>|[<span data-ttu-id="b8f30-184">printerLocation</span><span class="sxs-lookup"><span data-stu-id="b8f30-184">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="b8f30-185">打印机的物理和/或组织位置。</span><span class="sxs-lookup"><span data-stu-id="b8f30-185">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="b8f30-186">defaults</span><span class="sxs-lookup"><span data-stu-id="b8f30-186">defaults</span></span>|[<span data-ttu-id="b8f30-187">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="b8f30-187">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="b8f30-188">打印机的默认打印设置。</span><span class="sxs-lookup"><span data-stu-id="b8f30-188">The printer's default print settings.</span></span>|
|<span data-ttu-id="b8f30-189">capabilities</span><span class="sxs-lookup"><span data-stu-id="b8f30-189">capabilities</span></span>|[<span data-ttu-id="b8f30-190">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="b8f30-190">printerCapabilities</span></span>](printercapabilities.md)|<span data-ttu-id="b8f30-191">与此打印机共享关联的打印机的功能。</span><span class="sxs-lookup"><span data-stu-id="b8f30-191">The capabilities of the printer associated with this printer share.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8f30-192">关系</span><span class="sxs-lookup"><span data-stu-id="b8f30-192">Relationships</span></span>
| <span data-ttu-id="b8f30-193">关系</span><span class="sxs-lookup"><span data-stu-id="b8f30-193">Relationship</span></span> | <span data-ttu-id="b8f30-194">类型</span><span class="sxs-lookup"><span data-stu-id="b8f30-194">Type</span></span>        | <span data-ttu-id="b8f30-195">说明</span><span class="sxs-lookup"><span data-stu-id="b8f30-195">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b8f30-196">jobs</span><span class="sxs-lookup"><span data-stu-id="b8f30-196">jobs</span></span>|<span data-ttu-id="b8f30-197">[printJob](printjob.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b8f30-197">[printJob](printjob.md) collection</span></span>| <span data-ttu-id="b8f30-198">由打印机排入打印队列的作业列表。</span><span class="sxs-lookup"><span data-stu-id="b8f30-198">The list of jobs that are queued for printing by the printer.</span></span>|
|<span data-ttu-id="b8f30-199">shares</span><span class="sxs-lookup"><span data-stu-id="b8f30-199">shares</span></span>|<span data-ttu-id="b8f30-200">[printerShare](printershare.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b8f30-200">[printerShare](printershare.md) collection</span></span>| <span data-ttu-id="b8f30-201">与打印机关联的 printerShares 列表。</span><span class="sxs-lookup"><span data-stu-id="b8f30-201">The list of printerShares that are associated with the printer.</span></span> <span data-ttu-id="b8f30-202">目前，只能将一个 printerShare 与打印机关联。</span><span class="sxs-lookup"><span data-stu-id="b8f30-202">Currently, only one printerShare can be associated with the printer.</span></span> <span data-ttu-id="b8f30-203">只读。</span><span class="sxs-lookup"><span data-stu-id="b8f30-203">Read-only.</span></span> <span data-ttu-id="b8f30-204">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="b8f30-204">Nullable.</span></span>|
|<span data-ttu-id="b8f30-205">连接器</span><span class="sxs-lookup"><span data-stu-id="b8f30-205">connectors</span></span>|[<span data-ttu-id="b8f30-206">printConnector</span><span class="sxs-lookup"><span data-stu-id="b8f30-206">printConnector</span></span>](printconnector.md)|<span data-ttu-id="b8f30-207">与打印机关联的连接器。</span><span class="sxs-lookup"><span data-stu-id="b8f30-207">The connectors that are associated with the printer.</span></span>|
|<span data-ttu-id="b8f30-208">taskTriggers</span><span class="sxs-lookup"><span data-stu-id="b8f30-208">taskTriggers</span></span>|<span data-ttu-id="b8f30-209">[printTaskTrigger](printtasktrigger.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b8f30-209">[printTaskTrigger](printtasktrigger.md) collection</span></span>|<span data-ttu-id="b8f30-210">与打印机关联的任务触发器列表。</span><span class="sxs-lookup"><span data-stu-id="b8f30-210">A list of task triggers that are associated with the printer.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8f30-211">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b8f30-211">JSON representation</span></span>

<span data-ttu-id="b8f30-212">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8f30-212">The following is a JSON representation of the resource.</span></span>

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


