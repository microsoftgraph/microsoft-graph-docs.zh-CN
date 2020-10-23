---
title: 打印机资源类型
description: 表示已向通用打印服务注册的物理打印机设备。 打印机资源可用于管理打印作业、打印机设置、打印机元数据和注册状态。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: b86d3607decc8aca5b24b2be6f8344da87693fde
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48703571"
---
# <a name="printer-resource-type"></a><span data-ttu-id="af2cb-104">打印机资源类型</span><span class="sxs-lookup"><span data-stu-id="af2cb-104">printer resource type</span></span>

<span data-ttu-id="af2cb-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af2cb-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af2cb-106">表示已向通用打印服务注册的打印机设备。</span><span class="sxs-lookup"><span data-stu-id="af2cb-106">Represents a printer device that has been registered with the Universal Print service.</span></span> <span data-ttu-id="af2cb-107">打印机资源可用于管理打印作业、打印机设置、打印机元数据和注册状态。</span><span class="sxs-lookup"><span data-stu-id="af2cb-107">Printer resources can be used to manage print jobs, printer settings, printer metadata and registration status.</span></span>

## <a name="methods"></a><span data-ttu-id="af2cb-108">Methods</span><span class="sxs-lookup"><span data-stu-id="af2cb-108">Methods</span></span>

| <span data-ttu-id="af2cb-109">方法</span><span class="sxs-lookup"><span data-stu-id="af2cb-109">Method</span></span>       | <span data-ttu-id="af2cb-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="af2cb-110">Return Type</span></span> | <span data-ttu-id="af2cb-111">说明</span><span class="sxs-lookup"><span data-stu-id="af2cb-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="af2cb-112">创建</span><span class="sxs-lookup"><span data-stu-id="af2cb-112">Create</span></span>](../api/printer-create.md) | [<span data-ttu-id="af2cb-113">printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="af2cb-113">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="af2cb-114">创建 (注册) 具有通用打印的新打印机。</span><span class="sxs-lookup"><span data-stu-id="af2cb-114">Create (register) a new printer with Universal Print.</span></span> |
| [<span data-ttu-id="af2cb-115">获取</span><span class="sxs-lookup"><span data-stu-id="af2cb-115">Get</span></span>](../api/printer-get.md) | [<span data-ttu-id="af2cb-116">印刷</span><span class="sxs-lookup"><span data-stu-id="af2cb-116">printer</span></span>](printer.md) | <span data-ttu-id="af2cb-117">读取 printer 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="af2cb-117">Read the properties and relationships of the printer object.</span></span> |
| [<span data-ttu-id="af2cb-118">更新</span><span class="sxs-lookup"><span data-stu-id="af2cb-118">Update</span></span>](../api/printer-update.md) | [<span data-ttu-id="af2cb-119">印刷</span><span class="sxs-lookup"><span data-stu-id="af2cb-119">printer</span></span>](printer.md) | <span data-ttu-id="af2cb-120">更新 printer 对象。</span><span class="sxs-lookup"><span data-stu-id="af2cb-120">Update the printer object.</span></span> |
| [<span data-ttu-id="af2cb-121">删除</span><span class="sxs-lookup"><span data-stu-id="af2cb-121">Delete</span></span>](../api/printer-delete.md) | <span data-ttu-id="af2cb-122">无</span><span class="sxs-lookup"><span data-stu-id="af2cb-122">None</span></span> | <span data-ttu-id="af2cb-123">从通用打印服务注销物理打印机。</span><span class="sxs-lookup"><span data-stu-id="af2cb-123">Unregister the physical printer from the Universal Print service.</span></span> |
| [<span data-ttu-id="af2cb-124">restoreFactoryDefaults</span><span class="sxs-lookup"><span data-stu-id="af2cb-124">restoreFactoryDefaults</span></span>](../api/printer-restorefactorydefaults.md) | <span data-ttu-id="af2cb-125">无</span><span class="sxs-lookup"><span data-stu-id="af2cb-125">None</span></span> | <span data-ttu-id="af2cb-126">将打印机的默认设置还原为出厂默认设置。</span><span class="sxs-lookup"><span data-stu-id="af2cb-126">Restore a printer's defaults settings to factory defaults.</span></span> |
| [<span data-ttu-id="af2cb-127">列出作业</span><span class="sxs-lookup"><span data-stu-id="af2cb-127">List jobs</span></span>](../api/printer-list-jobs.md) | <span data-ttu-id="af2cb-128">[printJob](printjob.md) 集合</span><span class="sxs-lookup"><span data-stu-id="af2cb-128">[printJob](printjob.md) collection</span></span> | <span data-ttu-id="af2cb-129">获取排队等待打印机处理的打印作业的列表。</span><span class="sxs-lookup"><span data-stu-id="af2cb-129">Get a list of print jobs that are queued for processing by the printer.</span></span> |
| [<span data-ttu-id="af2cb-130">创建作业</span><span class="sxs-lookup"><span data-stu-id="af2cb-130">Create job</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="af2cb-131">printJob</span><span class="sxs-lookup"><span data-stu-id="af2cb-131">printJob</span></span>](printjob.md) | <span data-ttu-id="af2cb-132">为打印机创建一个新的打印作业。</span><span class="sxs-lookup"><span data-stu-id="af2cb-132">Create a new print job for the printer.</span></span> <span data-ttu-id="af2cb-133">若要开始打印作业，请使用 [start](../api/printjob-start.md)。</span><span class="sxs-lookup"><span data-stu-id="af2cb-133">To start printing the job, use [start](../api/printjob-start.md).</span></span> |
| [<span data-ttu-id="af2cb-134">List connectors</span><span class="sxs-lookup"><span data-stu-id="af2cb-134">List connectors</span></span>](../api/printer-list-connectors.md) | <span data-ttu-id="af2cb-135">[printConnector](printconnector.md) 集合</span><span class="sxs-lookup"><span data-stu-id="af2cb-135">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="af2cb-136">获取此打印机关联的连接器的列表。</span><span class="sxs-lookup"><span data-stu-id="af2cb-136">Get a list of connectors that this printer is associated with.</span></span> |
| [<span data-ttu-id="af2cb-137">List taskTriggers</span><span class="sxs-lookup"><span data-stu-id="af2cb-137">List taskTriggers</span></span>](../api/printer-list-tasktriggers.md) | <span data-ttu-id="af2cb-138">无</span><span class="sxs-lookup"><span data-stu-id="af2cb-138">None</span></span> | <span data-ttu-id="af2cb-139">列出与此打印机关联的 [printTaskTriggers](printtasktrigger.md) 。</span><span class="sxs-lookup"><span data-stu-id="af2cb-139">List [printTaskTriggers](printtasktrigger.md) associated with this printer.</span></span> |
| [<span data-ttu-id="af2cb-140">Create taskTrigger</span><span class="sxs-lookup"><span data-stu-id="af2cb-140">Create taskTrigger</span></span>](../api/printer-post-tasktriggers.md) | [<span data-ttu-id="af2cb-141">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="af2cb-141">printTaskTrigger</span></span>](printtasktrigger.md) | <span data-ttu-id="af2cb-142">创建在打印事件发生时运行的 [printTaskTrigger](printtasktrigger.md) 。</span><span class="sxs-lookup"><span data-stu-id="af2cb-142">Create a [printTaskTrigger](printtasktrigger.md) that runs when print events occur.</span></span> |
| [<span data-ttu-id="af2cb-143">Delete taskTrigger</span><span class="sxs-lookup"><span data-stu-id="af2cb-143">Delete taskTrigger</span></span>](../api/printer-delete-tasktrigger.md) | <span data-ttu-id="af2cb-144">无</span><span class="sxs-lookup"><span data-stu-id="af2cb-144">None</span></span> | <span data-ttu-id="af2cb-145">删除与打印机关联的 [printTaskTrigger](printtasktrigger.md) 。</span><span class="sxs-lookup"><span data-stu-id="af2cb-145">Delete a [printTaskTrigger](printtasktrigger.md) that is associated with the printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="af2cb-146">属性</span><span class="sxs-lookup"><span data-stu-id="af2cb-146">Properties</span></span>
| <span data-ttu-id="af2cb-147">属性</span><span class="sxs-lookup"><span data-stu-id="af2cb-147">Property</span></span>     | <span data-ttu-id="af2cb-148">类型</span><span class="sxs-lookup"><span data-stu-id="af2cb-148">Type</span></span>        | <span data-ttu-id="af2cb-149">说明</span><span class="sxs-lookup"><span data-stu-id="af2cb-149">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="af2cb-150">id</span><span class="sxs-lookup"><span data-stu-id="af2cb-150">id</span></span>|<span data-ttu-id="af2cb-151">String</span><span class="sxs-lookup"><span data-stu-id="af2cb-151">String</span></span>|<span data-ttu-id="af2cb-152">文档的标识符。</span><span class="sxs-lookup"><span data-stu-id="af2cb-152">The document's identifier.</span></span> <span data-ttu-id="af2cb-153">只读。</span><span class="sxs-lookup"><span data-stu-id="af2cb-153">Read-only.</span></span>|
|<span data-ttu-id="af2cb-154">displayName</span><span class="sxs-lookup"><span data-stu-id="af2cb-154">displayName</span></span>|<span data-ttu-id="af2cb-155">String</span><span class="sxs-lookup"><span data-stu-id="af2cb-155">String</span></span>|<span data-ttu-id="af2cb-156">打印机的名称。</span><span class="sxs-lookup"><span data-stu-id="af2cb-156">The name of the printer.</span></span>|
|<span data-ttu-id="af2cb-157">manufacturer</span><span class="sxs-lookup"><span data-stu-id="af2cb-157">manufacturer</span></span>|<span data-ttu-id="af2cb-158">String</span><span class="sxs-lookup"><span data-stu-id="af2cb-158">String</span></span>|<span data-ttu-id="af2cb-159">打印机报告的制造商。</span><span class="sxs-lookup"><span data-stu-id="af2cb-159">The manufacturer reported by the printer.</span></span> <span data-ttu-id="af2cb-160">只读。</span><span class="sxs-lookup"><span data-stu-id="af2cb-160">Read-only.</span></span>|
|<span data-ttu-id="af2cb-161">model</span><span class="sxs-lookup"><span data-stu-id="af2cb-161">model</span></span>|<span data-ttu-id="af2cb-162">String</span><span class="sxs-lookup"><span data-stu-id="af2cb-162">String</span></span>|<span data-ttu-id="af2cb-163">打印机报告的模型名称。</span><span class="sxs-lookup"><span data-stu-id="af2cb-163">The model name reported by the printer.</span></span> <span data-ttu-id="af2cb-164">只读。</span><span class="sxs-lookup"><span data-stu-id="af2cb-164">Read-only.</span></span>|
|<span data-ttu-id="af2cb-165">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="af2cb-165">registeredDateTime</span></span>|<span data-ttu-id="af2cb-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af2cb-166">DateTimeOffset</span></span>|<span data-ttu-id="af2cb-167">注册打印机时的 DateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="af2cb-167">The DateTimeOffset when the printer was registered.</span></span> <span data-ttu-id="af2cb-168">只读。</span><span class="sxs-lookup"><span data-stu-id="af2cb-168">Read-only.</span></span>|
|<span data-ttu-id="af2cb-169">status</span><span class="sxs-lookup"><span data-stu-id="af2cb-169">status</span></span>|[<span data-ttu-id="af2cb-170">printerStatus</span><span class="sxs-lookup"><span data-stu-id="af2cb-170">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="af2cb-171">打印机的处理状态，包括任何错误。</span><span class="sxs-lookup"><span data-stu-id="af2cb-171">The processing status of the printer, including any errors.</span></span> <span data-ttu-id="af2cb-172">只读。</span><span class="sxs-lookup"><span data-stu-id="af2cb-172">Read-only.</span></span>|
|<span data-ttu-id="af2cb-173">isShared</span><span class="sxs-lookup"><span data-stu-id="af2cb-173">isShared</span></span>|<span data-ttu-id="af2cb-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="af2cb-174">Boolean</span></span>|<span data-ttu-id="af2cb-175">如果打印机是共享的，则为 True;否则为 false。</span><span class="sxs-lookup"><span data-stu-id="af2cb-175">True if the printer is shared; false otherwise.</span></span> <span data-ttu-id="af2cb-176">只读。</span><span class="sxs-lookup"><span data-stu-id="af2cb-176">Read-only.</span></span>|
|<span data-ttu-id="af2cb-177">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="af2cb-177">isAcceptingJobs</span></span>|<span data-ttu-id="af2cb-178">布尔</span><span class="sxs-lookup"><span data-stu-id="af2cb-178">Boolean</span></span>|<span data-ttu-id="af2cb-179">打印机当前是否正在接受新的打印作业。</span><span class="sxs-lookup"><span data-stu-id="af2cb-179">Whether the printer is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="af2cb-180">location</span><span class="sxs-lookup"><span data-stu-id="af2cb-180">location</span></span>|[<span data-ttu-id="af2cb-181">printerLocation</span><span class="sxs-lookup"><span data-stu-id="af2cb-181">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="af2cb-182">打印机的物理和/或组织位置。</span><span class="sxs-lookup"><span data-stu-id="af2cb-182">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="af2cb-183">defaults</span><span class="sxs-lookup"><span data-stu-id="af2cb-183">defaults</span></span>|[<span data-ttu-id="af2cb-184">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="af2cb-184">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="af2cb-185">打印机的默认打印设置。</span><span class="sxs-lookup"><span data-stu-id="af2cb-185">The printer's default print settings.</span></span>|

## <a name="relationships"></a><span data-ttu-id="af2cb-186">关系</span><span class="sxs-lookup"><span data-stu-id="af2cb-186">Relationships</span></span>
| <span data-ttu-id="af2cb-187">关系</span><span class="sxs-lookup"><span data-stu-id="af2cb-187">Relationship</span></span> | <span data-ttu-id="af2cb-188">类型</span><span class="sxs-lookup"><span data-stu-id="af2cb-188">Type</span></span>        | <span data-ttu-id="af2cb-189">说明</span><span class="sxs-lookup"><span data-stu-id="af2cb-189">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="af2cb-190">jobs</span><span class="sxs-lookup"><span data-stu-id="af2cb-190">jobs</span></span>|<span data-ttu-id="af2cb-191">[printJob](printjob.md) 集合</span><span class="sxs-lookup"><span data-stu-id="af2cb-191">[printJob](printjob.md) collection</span></span>| <span data-ttu-id="af2cb-192">打印机排队等待打印的作业的列表。</span><span class="sxs-lookup"><span data-stu-id="af2cb-192">The list of jobs that are queued for printing by the printer.</span></span>|
|<span data-ttu-id="af2cb-193">shares</span><span class="sxs-lookup"><span data-stu-id="af2cb-193">shares</span></span>|<span data-ttu-id="af2cb-194">[printerShare](printershare.md) 集合</span><span class="sxs-lookup"><span data-stu-id="af2cb-194">[printerShare](printershare.md) collection</span></span>| <span data-ttu-id="af2cb-195">与打印机关联的 printerShares 的列表。</span><span class="sxs-lookup"><span data-stu-id="af2cb-195">The list of printerShares that are associated with the printer.</span></span> <span data-ttu-id="af2cb-196">目前，只有一个 printerShare 可以与打印机关联。</span><span class="sxs-lookup"><span data-stu-id="af2cb-196">Currently, only one printerShare can be associated with the printer.</span></span> <span data-ttu-id="af2cb-197">只读。</span><span class="sxs-lookup"><span data-stu-id="af2cb-197">Read-only.</span></span> <span data-ttu-id="af2cb-198">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="af2cb-198">Nullable.</span></span>|
|<span data-ttu-id="af2cb-199">插槽</span><span class="sxs-lookup"><span data-stu-id="af2cb-199">connectors</span></span>|[<span data-ttu-id="af2cb-200">printConnector</span><span class="sxs-lookup"><span data-stu-id="af2cb-200">printConnector</span></span>](printconnector.md)|<span data-ttu-id="af2cb-201">与打印机关联的连接器。</span><span class="sxs-lookup"><span data-stu-id="af2cb-201">The connectors that are associated with the printer.</span></span>|
|<span data-ttu-id="af2cb-202">taskTriggers</span><span class="sxs-lookup"><span data-stu-id="af2cb-202">taskTriggers</span></span>|<span data-ttu-id="af2cb-203">[printTaskTrigger](printtasktrigger.md) 集合</span><span class="sxs-lookup"><span data-stu-id="af2cb-203">[printTaskTrigger](printtasktrigger.md) collection</span></span>|<span data-ttu-id="af2cb-204">与打印机关联的任务触发器的列表。</span><span class="sxs-lookup"><span data-stu-id="af2cb-204">A list of task triggers that are associated with the printer.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="af2cb-205">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="af2cb-205">JSON representation</span></span>

<span data-ttu-id="af2cb-206">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af2cb-206">The following is a JSON representation of the resource.</span></span>

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
  "name": "String",
  "manufacturer": "String",
  "model": "String",
  "isShared": true,
  "registeredDateTime": "String (timestamp)",
  "acceptingJobs": true,
  "registeredBy": {"@odata.type": "microsoft.graph.printUserIdentity"},
  "location": {"@odata.type": "microsoft.graph.printerLocation"},
  "status": {"@odata.type": "microsoft.graph.printerStatus"},
  "defaults": {"@odata.type": "microsoft.graph.printerDefaults"}
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


