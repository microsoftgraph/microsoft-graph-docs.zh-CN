---
title: 打印机资源类型
description: 表示已向通用打印服务注册的物理打印机设备。 打印机资源可用于管理打印作业、打印机设置、打印机元数据和注册状态。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 255be26ed669e91248df1b007dc56b937ce2af98
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006882"
---
# <a name="printer-resource-type"></a><span data-ttu-id="d9629-104">打印机资源类型</span><span class="sxs-lookup"><span data-stu-id="d9629-104">printer resource type</span></span>

<span data-ttu-id="d9629-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9629-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9629-106">表示已向通用打印服务注册的物理打印机设备。</span><span class="sxs-lookup"><span data-stu-id="d9629-106">Represents a physical printer device that has been registered with the Universal Print service.</span></span> <span data-ttu-id="d9629-107">打印机资源可用于管理打印作业、打印机设置、打印机元数据和注册状态。</span><span class="sxs-lookup"><span data-stu-id="d9629-107">Printer resources can be used to manage print jobs, printer settings, printer metadata and registration status.</span></span>

## <a name="methods"></a><span data-ttu-id="d9629-108">方法</span><span class="sxs-lookup"><span data-stu-id="d9629-108">Methods</span></span>

| <span data-ttu-id="d9629-109">方法</span><span class="sxs-lookup"><span data-stu-id="d9629-109">Method</span></span>       | <span data-ttu-id="d9629-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d9629-110">Return Type</span></span> | <span data-ttu-id="d9629-111">说明</span><span class="sxs-lookup"><span data-stu-id="d9629-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d9629-112">创建</span><span class="sxs-lookup"><span data-stu-id="d9629-112">Create</span></span>](../api/printer-create.md) | [<span data-ttu-id="d9629-113">printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="d9629-113">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="d9629-114">创建（注册）具有通用打印的新打印机。</span><span class="sxs-lookup"><span data-stu-id="d9629-114">Create (register) a new printer with Universal Print.</span></span> |
| [<span data-ttu-id="d9629-115">获取</span><span class="sxs-lookup"><span data-stu-id="d9629-115">Get</span></span>](../api/printer-get.md) | [<span data-ttu-id="d9629-116">印刷</span><span class="sxs-lookup"><span data-stu-id="d9629-116">printer</span></span>](printer.md) | <span data-ttu-id="d9629-117">读取 printer 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d9629-117">Read the properties and relationships of the printer object.</span></span> |
| [<span data-ttu-id="d9629-118">更新</span><span class="sxs-lookup"><span data-stu-id="d9629-118">Update</span></span>](../api/printer-update.md) | [<span data-ttu-id="d9629-119">印刷</span><span class="sxs-lookup"><span data-stu-id="d9629-119">printer</span></span>](printer.md) | <span data-ttu-id="d9629-120">更新 printer 对象。</span><span class="sxs-lookup"><span data-stu-id="d9629-120">Update the printer object.</span></span> |
| [<span data-ttu-id="d9629-121">删除</span><span class="sxs-lookup"><span data-stu-id="d9629-121">Delete</span></span>](../api/printer-delete.md) | <span data-ttu-id="d9629-122">无</span><span class="sxs-lookup"><span data-stu-id="d9629-122">None</span></span> | <span data-ttu-id="d9629-123">在通用打印服务中注销物理 printerfrom。</span><span class="sxs-lookup"><span data-stu-id="d9629-123">Unregister the physical printerfrom the Universal Print service.</span></span> |
| [<span data-ttu-id="d9629-124">getCapabilities</span><span class="sxs-lookup"><span data-stu-id="d9629-124">getCapabilities</span></span>](../api/printer-getcapabilities.md) | [<span data-ttu-id="d9629-125">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="d9629-125">printerCapabilities</span></span>](printercapabilities.md) | <span data-ttu-id="d9629-126">获取打印机的功能列表。</span><span class="sxs-lookup"><span data-stu-id="d9629-126">Get a list of capabilities for the printer.</span></span> |
| [<span data-ttu-id="d9629-127">resetDefaults</span><span class="sxs-lookup"><span data-stu-id="d9629-127">resetDefaults</span></span>](../api/printer-resetdefaults.md) | <span data-ttu-id="d9629-128">无</span><span class="sxs-lookup"><span data-stu-id="d9629-128">None</span></span> | <span data-ttu-id="d9629-129">重置打印机的默认设置。</span><span class="sxs-lookup"><span data-stu-id="d9629-129">Reset a printer's default settings.</span></span> |
| [<span data-ttu-id="d9629-130">列出作业</span><span class="sxs-lookup"><span data-stu-id="d9629-130">List jobs</span></span>](../api/printer-list-jobs.md) | <span data-ttu-id="d9629-131">[printJob](printjob.md)集合</span><span class="sxs-lookup"><span data-stu-id="d9629-131">[printJob](printjob.md) collection</span></span> | <span data-ttu-id="d9629-132">获取排队等待打印机处理的打印作业的列表。</span><span class="sxs-lookup"><span data-stu-id="d9629-132">Get a list of print jobs that are queued for processing by the printer.</span></span> |
| [<span data-ttu-id="d9629-133">创建作业</span><span class="sxs-lookup"><span data-stu-id="d9629-133">Create job</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="d9629-134">printJob</span><span class="sxs-lookup"><span data-stu-id="d9629-134">printJob</span></span>](printjob.md) | <span data-ttu-id="d9629-135">为打印机创建一个新的打印作业。</span><span class="sxs-lookup"><span data-stu-id="d9629-135">Create a new print job for the printer.</span></span> <span data-ttu-id="d9629-136">若要开始打印作业，请使用[startPrintJob](../api/printjob-startprintjob.md)。</span><span class="sxs-lookup"><span data-stu-id="d9629-136">To start printing the job, use [startPrintJob](../api/printjob-startprintjob.md).</span></span> |
| [<span data-ttu-id="d9629-137">列出连接器</span><span class="sxs-lookup"><span data-stu-id="d9629-137">List connectors</span></span>](../api/printer-list-connectors.md) | <span data-ttu-id="d9629-138">[printConnector](printconnector.md)集合</span><span class="sxs-lookup"><span data-stu-id="d9629-138">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="d9629-139">获取此打印机关联的连接器的列表。</span><span class="sxs-lookup"><span data-stu-id="d9629-139">Get a list of connectors that this printer is associated with.</span></span> |
| [<span data-ttu-id="d9629-140">列出 allowedUsers</span><span class="sxs-lookup"><span data-stu-id="d9629-140">List allowedUsers</span></span>](../api/printer-list-allowedusers.md) | <span data-ttu-id="d9629-141">[printUserIdentity](printuseridentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="d9629-141">[printUserIdentity](printuseridentity.md) collection</span></span> | <span data-ttu-id="d9629-142">检索已授予访问权限以将打印作业提交到关联打印机的用户的列表。</span><span class="sxs-lookup"><span data-stu-id="d9629-142">Retrieve a list of users who have been granted access to submit print jobs to the associated printer.</span></span> |
| [<span data-ttu-id="d9629-143">添加 allowedUser</span><span class="sxs-lookup"><span data-stu-id="d9629-143">Add allowedUser</span></span>](../api/printer-post-allowedusers.md) | <span data-ttu-id="d9629-144">无</span><span class="sxs-lookup"><span data-stu-id="d9629-144">None</span></span> | <span data-ttu-id="d9629-145">向指定的用户授予向关联打印机提交打印作业的权限。</span><span class="sxs-lookup"><span data-stu-id="d9629-145">Grant the specified user access to submit print jobs to the associated printer.</span></span> |
| [<span data-ttu-id="d9629-146">删除 allowedUser</span><span class="sxs-lookup"><span data-stu-id="d9629-146">Remove allowedUser</span></span>](../api/printer-delete-alloweduser.md) | <span data-ttu-id="d9629-147">无</span><span class="sxs-lookup"><span data-stu-id="d9629-147">None</span></span> | <span data-ttu-id="d9629-148">撤销指定用户的打印机访问权限。</span><span class="sxs-lookup"><span data-stu-id="d9629-148">Revoke printer access from the specified user.</span></span> |
| [<span data-ttu-id="d9629-149">列出 allowedGroups</span><span class="sxs-lookup"><span data-stu-id="d9629-149">List allowedGroups</span></span>](../api/printer-list-allowedgroups.md) | <span data-ttu-id="d9629-150">[printIdentity](printidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="d9629-150">[printIdentity](printidentity.md) collection</span></span> | <span data-ttu-id="d9629-151">检索已向其授予将打印作业提交到关联打印机的访问权限的组列表。</span><span class="sxs-lookup"><span data-stu-id="d9629-151">Retrieve a list of groups which have been granted access to submit print jobs to the associated printer.</span></span> |
| [<span data-ttu-id="d9629-152">添加 allowedGroup</span><span class="sxs-lookup"><span data-stu-id="d9629-152">Add allowedGroup</span></span>](../api/printer-post-allowedgroups.md) | <span data-ttu-id="d9629-153">无</span><span class="sxs-lookup"><span data-stu-id="d9629-153">None</span></span> | <span data-ttu-id="d9629-154">向指定的组授予向关联打印机提交打印作业的权限。</span><span class="sxs-lookup"><span data-stu-id="d9629-154">Grant the specified group access to submit print jobs to the associated printer.</span></span> |
| [<span data-ttu-id="d9629-155">删除 allowedGroup</span><span class="sxs-lookup"><span data-stu-id="d9629-155">Remove allowedGroup</span></span>](../api/printer-delete-allowedgroup.md) | <span data-ttu-id="d9629-156">无</span><span class="sxs-lookup"><span data-stu-id="d9629-156">None</span></span> | <span data-ttu-id="d9629-157">撤销指定组的打印机访问权限。</span><span class="sxs-lookup"><span data-stu-id="d9629-157">Revoke printer access from the specified group.</span></span> |

## <a name="properties"></a><span data-ttu-id="d9629-158">属性</span><span class="sxs-lookup"><span data-stu-id="d9629-158">Properties</span></span>
| <span data-ttu-id="d9629-159">属性</span><span class="sxs-lookup"><span data-stu-id="d9629-159">Property</span></span>     | <span data-ttu-id="d9629-160">类型</span><span class="sxs-lookup"><span data-stu-id="d9629-160">Type</span></span>        | <span data-ttu-id="d9629-161">说明</span><span class="sxs-lookup"><span data-stu-id="d9629-161">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d9629-162">id</span><span class="sxs-lookup"><span data-stu-id="d9629-162">id</span></span>|<span data-ttu-id="d9629-163">String</span><span class="sxs-lookup"><span data-stu-id="d9629-163">String</span></span>|<span data-ttu-id="d9629-164">文档的标识符。</span><span class="sxs-lookup"><span data-stu-id="d9629-164">The document's identifier.</span></span> <span data-ttu-id="d9629-165">只读。</span><span class="sxs-lookup"><span data-stu-id="d9629-165">Read-only.</span></span>|
|<span data-ttu-id="d9629-166">displayName</span><span class="sxs-lookup"><span data-stu-id="d9629-166">displayName</span></span>|<span data-ttu-id="d9629-167">字符串</span><span class="sxs-lookup"><span data-stu-id="d9629-167">String</span></span>|<span data-ttu-id="d9629-168">打印机的名称。</span><span class="sxs-lookup"><span data-stu-id="d9629-168">The name of the printer.</span></span>|
|<span data-ttu-id="d9629-169">manufacturer</span><span class="sxs-lookup"><span data-stu-id="d9629-169">manufacturer</span></span>|<span data-ttu-id="d9629-170">String</span><span class="sxs-lookup"><span data-stu-id="d9629-170">String</span></span>|<span data-ttu-id="d9629-171">打印机报告的制造商。</span><span class="sxs-lookup"><span data-stu-id="d9629-171">The manufacturer reported by the printer.</span></span> <span data-ttu-id="d9629-172">只读。</span><span class="sxs-lookup"><span data-stu-id="d9629-172">Read-only.</span></span>|
|<span data-ttu-id="d9629-173">model</span><span class="sxs-lookup"><span data-stu-id="d9629-173">model</span></span>|<span data-ttu-id="d9629-174">String</span><span class="sxs-lookup"><span data-stu-id="d9629-174">String</span></span>|<span data-ttu-id="d9629-175">打印机报告的模型名称。</span><span class="sxs-lookup"><span data-stu-id="d9629-175">The model name reported by the printer.</span></span> <span data-ttu-id="d9629-176">只读。</span><span class="sxs-lookup"><span data-stu-id="d9629-176">Read-only.</span></span>|
|<span data-ttu-id="d9629-177">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="d9629-177">registeredDateTime</span></span>|<span data-ttu-id="d9629-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9629-178">DateTimeOffset</span></span>|<span data-ttu-id="d9629-179">注册打印机时的 DateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="d9629-179">The DateTimeOffset when the printer was registered.</span></span> <span data-ttu-id="d9629-180">只读。</span><span class="sxs-lookup"><span data-stu-id="d9629-180">Read-only.</span></span>|
|<span data-ttu-id="d9629-181">status</span><span class="sxs-lookup"><span data-stu-id="d9629-181">status</span></span>|[<span data-ttu-id="d9629-182">printerStatus</span><span class="sxs-lookup"><span data-stu-id="d9629-182">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="d9629-183">打印机的处理状态，包括任何错误。</span><span class="sxs-lookup"><span data-stu-id="d9629-183">The processing status of the printer, including any errors.</span></span> <span data-ttu-id="d9629-184">只读。</span><span class="sxs-lookup"><span data-stu-id="d9629-184">Read-only.</span></span>|
|<span data-ttu-id="d9629-185">isShared</span><span class="sxs-lookup"><span data-stu-id="d9629-185">isShared</span></span>|<span data-ttu-id="d9629-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9629-186">Boolean</span></span>|<span data-ttu-id="d9629-187">如果打印机是共享的，则为 True;否则为 false。</span><span class="sxs-lookup"><span data-stu-id="d9629-187">True if the printer is shared; false otherwise.</span></span> <span data-ttu-id="d9629-188">只读。</span><span class="sxs-lookup"><span data-stu-id="d9629-188">Read-only.</span></span>|
|<span data-ttu-id="d9629-189">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="d9629-189">isAcceptingJobs</span></span>|<span data-ttu-id="d9629-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9629-190">Boolean</span></span>|<span data-ttu-id="d9629-191">打印机当前是否正在接受新的打印作业。</span><span class="sxs-lookup"><span data-stu-id="d9629-191">Whether the printer is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="d9629-192">位置</span><span class="sxs-lookup"><span data-stu-id="d9629-192">location</span></span>|[<span data-ttu-id="d9629-193">printerLocation</span><span class="sxs-lookup"><span data-stu-id="d9629-193">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="d9629-194">打印机的物理和/或组织位置。</span><span class="sxs-lookup"><span data-stu-id="d9629-194">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="d9629-195">缺省值</span><span class="sxs-lookup"><span data-stu-id="d9629-195">defaults</span></span>|[<span data-ttu-id="d9629-196">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="d9629-196">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="d9629-197">打印机的默认打印设置。</span><span class="sxs-lookup"><span data-stu-id="d9629-197">The printer's default print settings.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9629-198">关系</span><span class="sxs-lookup"><span data-stu-id="d9629-198">Relationships</span></span>
| <span data-ttu-id="d9629-199">关系</span><span class="sxs-lookup"><span data-stu-id="d9629-199">Relationship</span></span> | <span data-ttu-id="d9629-200">类型</span><span class="sxs-lookup"><span data-stu-id="d9629-200">Type</span></span>        | <span data-ttu-id="d9629-201">说明</span><span class="sxs-lookup"><span data-stu-id="d9629-201">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d9629-202">jobs</span><span class="sxs-lookup"><span data-stu-id="d9629-202">jobs</span></span>|<span data-ttu-id="d9629-203">[printJob](printjob.md)集合</span><span class="sxs-lookup"><span data-stu-id="d9629-203">[printJob](printjob.md) collection</span></span>| <span data-ttu-id="d9629-204">打印机排队等待打印的作业的列表。</span><span class="sxs-lookup"><span data-stu-id="d9629-204">The list of jobs that are queued for printing by the printer.</span></span>|
|<span data-ttu-id="d9629-205">shares</span><span class="sxs-lookup"><span data-stu-id="d9629-205">shares</span></span>|<span data-ttu-id="d9629-206">[printerShare](printershare.md)集合</span><span class="sxs-lookup"><span data-stu-id="d9629-206">[printerShare](printershare.md) collection</span></span>| <span data-ttu-id="d9629-207">与打印机关联的 printerShares 的列表。</span><span class="sxs-lookup"><span data-stu-id="d9629-207">The list of printerShares that are associated with the printer.</span></span> <span data-ttu-id="d9629-208">只读。</span><span class="sxs-lookup"><span data-stu-id="d9629-208">Read-only.</span></span> <span data-ttu-id="d9629-209">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="d9629-209">Nullable.</span></span>|
|<span data-ttu-id="d9629-210">插槽</span><span class="sxs-lookup"><span data-stu-id="d9629-210">connectors</span></span>|[<span data-ttu-id="d9629-211">printConnector</span><span class="sxs-lookup"><span data-stu-id="d9629-211">printConnector</span></span>](printconnector.md)|<span data-ttu-id="d9629-212">与打印机关联的连接器。</span><span class="sxs-lookup"><span data-stu-id="d9629-212">The connectors that are associated with the printer.</span></span>|
|<span data-ttu-id="d9629-213">allowedUsers</span><span class="sxs-lookup"><span data-stu-id="d9629-213">allowedUsers</span></span>|<span data-ttu-id="d9629-214">[printUserIdentity](printuseridentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="d9629-214">[printUserIdentity](printuseridentity.md) collection</span></span>|<span data-ttu-id="d9629-215">有权使用打印机打印的用户。</span><span class="sxs-lookup"><span data-stu-id="d9629-215">The users who have access to print using the printer.</span></span>|
|<span data-ttu-id="d9629-216">allowedGroups</span><span class="sxs-lookup"><span data-stu-id="d9629-216">allowedGroups</span></span>|[<span data-ttu-id="d9629-217">printIdentity</span><span class="sxs-lookup"><span data-stu-id="d9629-217">printIdentity</span></span>](printidentity.md)|<span data-ttu-id="d9629-218">其用户有权使用打印机打印的组。</span><span class="sxs-lookup"><span data-stu-id="d9629-218">The groups whose users have access to print using the printer.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d9629-219">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d9629-219">JSON representation</span></span>

<span data-ttu-id="d9629-220">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9629-220">The following is a JSON representation of the resource.</span></span>

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
