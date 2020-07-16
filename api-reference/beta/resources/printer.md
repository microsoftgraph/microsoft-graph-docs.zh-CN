---
title: 打印机资源类型
description: 表示已向通用打印服务注册的物理打印机设备。 打印机资源可用于管理打印作业、打印机设置、打印机元数据和注册状态。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 6573f17753a3c9b487324def9973bddd0759ed4b
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091436"
---
# <a name="printer-resource-type"></a><span data-ttu-id="8a568-104">打印机资源类型</span><span class="sxs-lookup"><span data-stu-id="8a568-104">printer resource type</span></span>

<span data-ttu-id="8a568-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a568-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a568-106">表示已向通用打印服务注册的物理打印机设备。</span><span class="sxs-lookup"><span data-stu-id="8a568-106">Represents a physical printer device that has been registered with the Universal Print service.</span></span> <span data-ttu-id="8a568-107">打印机资源可用于管理打印作业、打印机设置、打印机元数据和注册状态。</span><span class="sxs-lookup"><span data-stu-id="8a568-107">Printer resources can be used to manage print jobs, printer settings, printer metadata and registration status.</span></span>

## <a name="methods"></a><span data-ttu-id="8a568-108">方法</span><span class="sxs-lookup"><span data-stu-id="8a568-108">Methods</span></span>

| <span data-ttu-id="8a568-109">方法</span><span class="sxs-lookup"><span data-stu-id="8a568-109">Method</span></span>       | <span data-ttu-id="8a568-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="8a568-110">Return Type</span></span> | <span data-ttu-id="8a568-111">说明</span><span class="sxs-lookup"><span data-stu-id="8a568-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8a568-112">创建</span><span class="sxs-lookup"><span data-stu-id="8a568-112">Create</span></span>](../api/printer-create.md) | [<span data-ttu-id="8a568-113">printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="8a568-113">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="8a568-114">创建 (注册) 具有通用打印的新打印机。</span><span class="sxs-lookup"><span data-stu-id="8a568-114">Create (register) a new printer with Universal Print.</span></span> |
| [<span data-ttu-id="8a568-115">获取</span><span class="sxs-lookup"><span data-stu-id="8a568-115">Get</span></span>](../api/printer-get.md) | [<span data-ttu-id="8a568-116">印刷</span><span class="sxs-lookup"><span data-stu-id="8a568-116">printer</span></span>](printer.md) | <span data-ttu-id="8a568-117">读取 printer 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8a568-117">Read the properties and relationships of the printer object.</span></span> |
| [<span data-ttu-id="8a568-118">更新</span><span class="sxs-lookup"><span data-stu-id="8a568-118">Update</span></span>](../api/printer-update.md) | [<span data-ttu-id="8a568-119">印刷</span><span class="sxs-lookup"><span data-stu-id="8a568-119">printer</span></span>](printer.md) | <span data-ttu-id="8a568-120">更新 printer 对象。</span><span class="sxs-lookup"><span data-stu-id="8a568-120">Update the printer object.</span></span> |
| [<span data-ttu-id="8a568-121">删除</span><span class="sxs-lookup"><span data-stu-id="8a568-121">Delete</span></span>](../api/printer-delete.md) | <span data-ttu-id="8a568-122">无</span><span class="sxs-lookup"><span data-stu-id="8a568-122">None</span></span> | <span data-ttu-id="8a568-123">在通用打印服务中注销物理 printerfrom。</span><span class="sxs-lookup"><span data-stu-id="8a568-123">Unregister the physical printerfrom the Universal Print service.</span></span> |
| [<span data-ttu-id="8a568-124">getCapabilities</span><span class="sxs-lookup"><span data-stu-id="8a568-124">getCapabilities</span></span>](../api/printer-getcapabilities.md) | [<span data-ttu-id="8a568-125">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="8a568-125">printerCapabilities</span></span>](printercapabilities.md) | <span data-ttu-id="8a568-126">获取打印机的功能列表。</span><span class="sxs-lookup"><span data-stu-id="8a568-126">Get a list of capabilities for the printer.</span></span> |
| [<span data-ttu-id="8a568-127">resetDefaults</span><span class="sxs-lookup"><span data-stu-id="8a568-127">resetDefaults</span></span>](../api/printer-resetdefaults.md) | <span data-ttu-id="8a568-128">无</span><span class="sxs-lookup"><span data-stu-id="8a568-128">None</span></span> | <span data-ttu-id="8a568-129">重置打印机的默认设置。</span><span class="sxs-lookup"><span data-stu-id="8a568-129">Reset a printer's default settings.</span></span> |
| [<span data-ttu-id="8a568-130">列出作业</span><span class="sxs-lookup"><span data-stu-id="8a568-130">List jobs</span></span>](../api/printer-list-jobs.md) | <span data-ttu-id="8a568-131">[printJob](printjob.md)集合</span><span class="sxs-lookup"><span data-stu-id="8a568-131">[printJob](printjob.md) collection</span></span> | <span data-ttu-id="8a568-132">获取排队等待打印机处理的打印作业的列表。</span><span class="sxs-lookup"><span data-stu-id="8a568-132">Get a list of print jobs that are queued for processing by the printer.</span></span> |
| [<span data-ttu-id="8a568-133">创建作业</span><span class="sxs-lookup"><span data-stu-id="8a568-133">Create job</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="8a568-134">printJob</span><span class="sxs-lookup"><span data-stu-id="8a568-134">printJob</span></span>](printjob.md) | <span data-ttu-id="8a568-135">为打印机创建一个新的打印作业。</span><span class="sxs-lookup"><span data-stu-id="8a568-135">Create a new print job for the printer.</span></span> <span data-ttu-id="8a568-136">若要开始打印作业，请使用[startPrintJob](../api/printjob-startprintjob.md)。</span><span class="sxs-lookup"><span data-stu-id="8a568-136">To start printing the job, use [startPrintJob](../api/printjob-startprintjob.md).</span></span> |
| [<span data-ttu-id="8a568-137">列出连接器</span><span class="sxs-lookup"><span data-stu-id="8a568-137">List connectors</span></span>](../api/printer-list-connectors.md) | <span data-ttu-id="8a568-138">[printConnector](printconnector.md)集合</span><span class="sxs-lookup"><span data-stu-id="8a568-138">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="8a568-139">获取此打印机关联的连接器的列表。</span><span class="sxs-lookup"><span data-stu-id="8a568-139">Get a list of connectors that this printer is associated with.</span></span> |
| [<span data-ttu-id="8a568-140">列出 allowedUsers</span><span class="sxs-lookup"><span data-stu-id="8a568-140">List allowedUsers</span></span>](../api/printer-list-allowedusers.md) | <span data-ttu-id="8a568-141">[printUserIdentity](printuseridentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="8a568-141">[printUserIdentity](printuseridentity.md) collection</span></span> | <span data-ttu-id="8a568-142">检索已授予访问权限以将打印作业提交到关联打印机的用户的列表。</span><span class="sxs-lookup"><span data-stu-id="8a568-142">Retrieve a list of users who have been granted access to submit print jobs to the associated printer.</span></span> |
| [<span data-ttu-id="8a568-143">添加 allowedUser</span><span class="sxs-lookup"><span data-stu-id="8a568-143">Add allowedUser</span></span>](../api/printer-post-allowedusers.md) | <span data-ttu-id="8a568-144">无</span><span class="sxs-lookup"><span data-stu-id="8a568-144">None</span></span> | <span data-ttu-id="8a568-145">向指定的用户授予向关联打印机提交打印作业的权限。</span><span class="sxs-lookup"><span data-stu-id="8a568-145">Grant the specified user access to submit print jobs to the associated printer.</span></span> |
| [<span data-ttu-id="8a568-146">删除 allowedUser</span><span class="sxs-lookup"><span data-stu-id="8a568-146">Remove allowedUser</span></span>](../api/printer-delete-alloweduser.md) | <span data-ttu-id="8a568-147">无</span><span class="sxs-lookup"><span data-stu-id="8a568-147">None</span></span> | <span data-ttu-id="8a568-148">撤销指定用户的打印机访问权限。</span><span class="sxs-lookup"><span data-stu-id="8a568-148">Revoke printer access from the specified user.</span></span> |
| [<span data-ttu-id="8a568-149">列出 allowedGroups</span><span class="sxs-lookup"><span data-stu-id="8a568-149">List allowedGroups</span></span>](../api/printer-list-allowedgroups.md) | <span data-ttu-id="8a568-150">[printIdentity](printidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="8a568-150">[printIdentity](printidentity.md) collection</span></span> | <span data-ttu-id="8a568-151">检索已向其授予将打印作业提交到关联打印机的访问权限的组列表。</span><span class="sxs-lookup"><span data-stu-id="8a568-151">Retrieve a list of groups which have been granted access to submit print jobs to the associated printer.</span></span> |
| [<span data-ttu-id="8a568-152">添加 allowedGroup</span><span class="sxs-lookup"><span data-stu-id="8a568-152">Add allowedGroup</span></span>](../api/printer-post-allowedgroups.md) | <span data-ttu-id="8a568-153">无</span><span class="sxs-lookup"><span data-stu-id="8a568-153">None</span></span> | <span data-ttu-id="8a568-154">向指定的组授予向关联打印机提交打印作业的权限。</span><span class="sxs-lookup"><span data-stu-id="8a568-154">Grant the specified group access to submit print jobs to the associated printer.</span></span> |
| [<span data-ttu-id="8a568-155">删除 allowedGroup</span><span class="sxs-lookup"><span data-stu-id="8a568-155">Remove allowedGroup</span></span>](../api/printer-delete-allowedgroup.md) | <span data-ttu-id="8a568-156">无</span><span class="sxs-lookup"><span data-stu-id="8a568-156">None</span></span> | <span data-ttu-id="8a568-157">撤销指定组的打印机访问权限。</span><span class="sxs-lookup"><span data-stu-id="8a568-157">Revoke printer access from the specified group.</span></span> |
| [<span data-ttu-id="8a568-158">列出 taskTriggers</span><span class="sxs-lookup"><span data-stu-id="8a568-158">List taskTriggers</span></span>](../api/printer-list-tasktriggers.md) | <span data-ttu-id="8a568-159">无</span><span class="sxs-lookup"><span data-stu-id="8a568-159">None</span></span> | <span data-ttu-id="8a568-160">列出与此打印机关联的[printTaskTriggers](printtasktrigger.md) 。</span><span class="sxs-lookup"><span data-stu-id="8a568-160">List [printTaskTriggers](printtasktrigger.md) associated with this printer.</span></span> |
| [<span data-ttu-id="8a568-161">创建 taskTrigger</span><span class="sxs-lookup"><span data-stu-id="8a568-161">Create taskTrigger</span></span>](../api/printer-post-tasktriggers.md) | [<span data-ttu-id="8a568-162">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="8a568-162">printTaskTrigger</span></span>](printtasktrigger.md) | <span data-ttu-id="8a568-163">创建在打印事件发生时运行的[printTaskTrigger](printtasktrigger.md) 。</span><span class="sxs-lookup"><span data-stu-id="8a568-163">Create a [printTaskTrigger](printtasktrigger.md) that runs when print events occur.</span></span> |
| [<span data-ttu-id="8a568-164">删除 taskTrigger</span><span class="sxs-lookup"><span data-stu-id="8a568-164">Delete taskTrigger</span></span>](../api/printer-delete-tasktrigger.md) | <span data-ttu-id="8a568-165">无</span><span class="sxs-lookup"><span data-stu-id="8a568-165">None</span></span> | <span data-ttu-id="8a568-166">删除与打印机关联的[printTaskTrigger](printtasktrigger.md) 。</span><span class="sxs-lookup"><span data-stu-id="8a568-166">Delete a [printTaskTrigger](printtasktrigger.md) that is associated with the printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="8a568-167">属性</span><span class="sxs-lookup"><span data-stu-id="8a568-167">Properties</span></span>
| <span data-ttu-id="8a568-168">属性</span><span class="sxs-lookup"><span data-stu-id="8a568-168">Property</span></span>     | <span data-ttu-id="8a568-169">类型</span><span class="sxs-lookup"><span data-stu-id="8a568-169">Type</span></span>        | <span data-ttu-id="8a568-170">说明</span><span class="sxs-lookup"><span data-stu-id="8a568-170">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8a568-171">id</span><span class="sxs-lookup"><span data-stu-id="8a568-171">id</span></span>|<span data-ttu-id="8a568-172">String</span><span class="sxs-lookup"><span data-stu-id="8a568-172">String</span></span>|<span data-ttu-id="8a568-173">文档的标识符。</span><span class="sxs-lookup"><span data-stu-id="8a568-173">The document's identifier.</span></span> <span data-ttu-id="8a568-174">只读。</span><span class="sxs-lookup"><span data-stu-id="8a568-174">Read-only.</span></span>|
|<span data-ttu-id="8a568-175">displayName</span><span class="sxs-lookup"><span data-stu-id="8a568-175">displayName</span></span>|<span data-ttu-id="8a568-176">字符串</span><span class="sxs-lookup"><span data-stu-id="8a568-176">String</span></span>|<span data-ttu-id="8a568-177">打印机的名称。</span><span class="sxs-lookup"><span data-stu-id="8a568-177">The name of the printer.</span></span>|
|<span data-ttu-id="8a568-178">manufacturer</span><span class="sxs-lookup"><span data-stu-id="8a568-178">manufacturer</span></span>|<span data-ttu-id="8a568-179">String</span><span class="sxs-lookup"><span data-stu-id="8a568-179">String</span></span>|<span data-ttu-id="8a568-180">打印机报告的制造商。</span><span class="sxs-lookup"><span data-stu-id="8a568-180">The manufacturer reported by the printer.</span></span> <span data-ttu-id="8a568-181">只读。</span><span class="sxs-lookup"><span data-stu-id="8a568-181">Read-only.</span></span>|
|<span data-ttu-id="8a568-182">model</span><span class="sxs-lookup"><span data-stu-id="8a568-182">model</span></span>|<span data-ttu-id="8a568-183">String</span><span class="sxs-lookup"><span data-stu-id="8a568-183">String</span></span>|<span data-ttu-id="8a568-184">打印机报告的模型名称。</span><span class="sxs-lookup"><span data-stu-id="8a568-184">The model name reported by the printer.</span></span> <span data-ttu-id="8a568-185">只读。</span><span class="sxs-lookup"><span data-stu-id="8a568-185">Read-only.</span></span>|
|<span data-ttu-id="8a568-186">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="8a568-186">registeredDateTime</span></span>|<span data-ttu-id="8a568-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a568-187">DateTimeOffset</span></span>|<span data-ttu-id="8a568-188">注册打印机时的 DateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="8a568-188">The DateTimeOffset when the printer was registered.</span></span> <span data-ttu-id="8a568-189">只读。</span><span class="sxs-lookup"><span data-stu-id="8a568-189">Read-only.</span></span>|
|<span data-ttu-id="8a568-190">status</span><span class="sxs-lookup"><span data-stu-id="8a568-190">status</span></span>|[<span data-ttu-id="8a568-191">printerStatus</span><span class="sxs-lookup"><span data-stu-id="8a568-191">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="8a568-192">打印机的处理状态，包括任何错误。</span><span class="sxs-lookup"><span data-stu-id="8a568-192">The processing status of the printer, including any errors.</span></span> <span data-ttu-id="8a568-193">只读。</span><span class="sxs-lookup"><span data-stu-id="8a568-193">Read-only.</span></span>|
|<span data-ttu-id="8a568-194">isShared</span><span class="sxs-lookup"><span data-stu-id="8a568-194">isShared</span></span>|<span data-ttu-id="8a568-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a568-195">Boolean</span></span>|<span data-ttu-id="8a568-196">如果打印机是共享的，则为 True;否则为 false。</span><span class="sxs-lookup"><span data-stu-id="8a568-196">True if the printer is shared; false otherwise.</span></span> <span data-ttu-id="8a568-197">只读。</span><span class="sxs-lookup"><span data-stu-id="8a568-197">Read-only.</span></span>|
|<span data-ttu-id="8a568-198">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="8a568-198">isAcceptingJobs</span></span>|<span data-ttu-id="8a568-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a568-199">Boolean</span></span>|<span data-ttu-id="8a568-200">打印机当前是否正在接受新的打印作业。</span><span class="sxs-lookup"><span data-stu-id="8a568-200">Whether the printer is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="8a568-201">位置</span><span class="sxs-lookup"><span data-stu-id="8a568-201">location</span></span>|[<span data-ttu-id="8a568-202">printerLocation</span><span class="sxs-lookup"><span data-stu-id="8a568-202">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="8a568-203">打印机的物理和/或组织位置。</span><span class="sxs-lookup"><span data-stu-id="8a568-203">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="8a568-204">缺省值</span><span class="sxs-lookup"><span data-stu-id="8a568-204">defaults</span></span>|[<span data-ttu-id="8a568-205">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="8a568-205">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="8a568-206">打印机的默认打印设置。</span><span class="sxs-lookup"><span data-stu-id="8a568-206">The printer's default print settings.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a568-207">关系</span><span class="sxs-lookup"><span data-stu-id="8a568-207">Relationships</span></span>
| <span data-ttu-id="8a568-208">关系</span><span class="sxs-lookup"><span data-stu-id="8a568-208">Relationship</span></span> | <span data-ttu-id="8a568-209">类型</span><span class="sxs-lookup"><span data-stu-id="8a568-209">Type</span></span>        | <span data-ttu-id="8a568-210">说明</span><span class="sxs-lookup"><span data-stu-id="8a568-210">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8a568-211">jobs</span><span class="sxs-lookup"><span data-stu-id="8a568-211">jobs</span></span>|<span data-ttu-id="8a568-212">[printJob](printjob.md)集合</span><span class="sxs-lookup"><span data-stu-id="8a568-212">[printJob](printjob.md) collection</span></span>| <span data-ttu-id="8a568-213">打印机排队等待打印的作业的列表。</span><span class="sxs-lookup"><span data-stu-id="8a568-213">The list of jobs that are queued for printing by the printer.</span></span>|
|<span data-ttu-id="8a568-214">shares</span><span class="sxs-lookup"><span data-stu-id="8a568-214">shares</span></span>|<span data-ttu-id="8a568-215">[printerShare](printershare.md)集合</span><span class="sxs-lookup"><span data-stu-id="8a568-215">[printerShare](printershare.md) collection</span></span>| <span data-ttu-id="8a568-216">与打印机关联的 printerShares 的列表。</span><span class="sxs-lookup"><span data-stu-id="8a568-216">The list of printerShares that are associated with the printer.</span></span> <span data-ttu-id="8a568-217">只读。</span><span class="sxs-lookup"><span data-stu-id="8a568-217">Read-only.</span></span> <span data-ttu-id="8a568-218">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="8a568-218">Nullable.</span></span>|
|<span data-ttu-id="8a568-219">插槽</span><span class="sxs-lookup"><span data-stu-id="8a568-219">connectors</span></span>|[<span data-ttu-id="8a568-220">printConnector</span><span class="sxs-lookup"><span data-stu-id="8a568-220">printConnector</span></span>](printconnector.md)|<span data-ttu-id="8a568-221">与打印机关联的连接器。</span><span class="sxs-lookup"><span data-stu-id="8a568-221">The connectors that are associated with the printer.</span></span>|
|<span data-ttu-id="8a568-222">allowedUsers</span><span class="sxs-lookup"><span data-stu-id="8a568-222">allowedUsers</span></span>|<span data-ttu-id="8a568-223">[printUserIdentity](printuseridentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="8a568-223">[printUserIdentity](printuseridentity.md) collection</span></span>|<span data-ttu-id="8a568-224">有权使用打印机打印的用户。</span><span class="sxs-lookup"><span data-stu-id="8a568-224">The users who have access to print using the printer.</span></span>|
|<span data-ttu-id="8a568-225">allowedGroups</span><span class="sxs-lookup"><span data-stu-id="8a568-225">allowedGroups</span></span>|[<span data-ttu-id="8a568-226">printIdentity</span><span class="sxs-lookup"><span data-stu-id="8a568-226">printIdentity</span></span>](printidentity.md)|<span data-ttu-id="8a568-227">其用户有权使用打印机打印的组。</span><span class="sxs-lookup"><span data-stu-id="8a568-227">The groups whose users have access to print using the printer.</span></span>|
|<span data-ttu-id="8a568-228">taskTriggers</span><span class="sxs-lookup"><span data-stu-id="8a568-228">taskTriggers</span></span>|<span data-ttu-id="8a568-229">[printTaskTrigger](printtasktrigger.md)集合</span><span class="sxs-lookup"><span data-stu-id="8a568-229">[printTaskTrigger](printtasktrigger.md) collection</span></span>|<span data-ttu-id="8a568-230">与打印机关联的任务触发器的列表。</span><span class="sxs-lookup"><span data-stu-id="8a568-230">A list of task triggers that are associated with the printer.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8a568-231">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8a568-231">JSON representation</span></span>

<span data-ttu-id="8a568-232">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a568-232">The following is a JSON representation of the resource.</span></span>

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
