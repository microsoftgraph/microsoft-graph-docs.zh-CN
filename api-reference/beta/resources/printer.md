---
title: 打印机资源类型
description: 表示已向通用打印服务注册的物理打印机设备。 打印机资源可用于管理打印作业、打印机设置、打印机元数据和注册状态。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: ce7bf6140b831c3e911ebb744106840ae8e027a8
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44217078"
---
# <a name="printer-resource-type"></a><span data-ttu-id="7bf84-104">打印机资源类型</span><span class="sxs-lookup"><span data-stu-id="7bf84-104">printer resource type</span></span>

<span data-ttu-id="7bf84-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bf84-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bf84-106">表示已向通用打印服务注册的物理打印机设备。</span><span class="sxs-lookup"><span data-stu-id="7bf84-106">Represents a physical printer device that has been registered with the Universal Print service.</span></span> <span data-ttu-id="7bf84-107">打印机资源可用于管理打印作业、打印机设置、打印机元数据和注册状态。</span><span class="sxs-lookup"><span data-stu-id="7bf84-107">Printer resources can be used to manage print jobs, printer settings, printer metadata and registration status.</span></span>

## <a name="methods"></a><span data-ttu-id="7bf84-108">Methods</span><span class="sxs-lookup"><span data-stu-id="7bf84-108">Methods</span></span>

| <span data-ttu-id="7bf84-109">方法</span><span class="sxs-lookup"><span data-stu-id="7bf84-109">Method</span></span>       | <span data-ttu-id="7bf84-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="7bf84-110">Return Type</span></span> | <span data-ttu-id="7bf84-111">说明</span><span class="sxs-lookup"><span data-stu-id="7bf84-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="7bf84-112">获取打印机</span><span class="sxs-lookup"><span data-stu-id="7bf84-112">Get printer</span></span>](../api/printer-get.md) | [<span data-ttu-id="7bf84-113">印刷</span><span class="sxs-lookup"><span data-stu-id="7bf84-113">printer</span></span>](printer.md) | <span data-ttu-id="7bf84-114">读取 printer 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7bf84-114">Read the properties and relationships of the printer object.</span></span> |
| [<span data-ttu-id="7bf84-115">更新</span><span class="sxs-lookup"><span data-stu-id="7bf84-115">Update</span></span>](../api/printer-update.md) | [<span data-ttu-id="7bf84-116">印刷</span><span class="sxs-lookup"><span data-stu-id="7bf84-116">printer</span></span>](printer.md) | <span data-ttu-id="7bf84-117">更新 printer 对象。</span><span class="sxs-lookup"><span data-stu-id="7bf84-117">Update the printer object.</span></span> |
| [<span data-ttu-id="7bf84-118">删除</span><span class="sxs-lookup"><span data-stu-id="7bf84-118">Delete</span></span>](../api/printer-delete.md) | <span data-ttu-id="7bf84-119">无</span><span class="sxs-lookup"><span data-stu-id="7bf84-119">None</span></span> | <span data-ttu-id="7bf84-120">在通用打印服务中注销物理 printerfrom。</span><span class="sxs-lookup"><span data-stu-id="7bf84-120">Unregister the physical printerfrom the Universal Print service.</span></span> |
| [<span data-ttu-id="7bf84-121">getCapabilities</span><span class="sxs-lookup"><span data-stu-id="7bf84-121">getCapabilities</span></span>](../api/printer-getcapabilities.md) | [<span data-ttu-id="7bf84-122">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="7bf84-122">printerCapabilities</span></span>](printercapabilities.md) | <span data-ttu-id="7bf84-123">获取打印机的功能列表。</span><span class="sxs-lookup"><span data-stu-id="7bf84-123">Get a list of capabilities for the printer.</span></span> |
| [<span data-ttu-id="7bf84-124">resetDefaults</span><span class="sxs-lookup"><span data-stu-id="7bf84-124">resetDefaults</span></span>](../api/printer-resetdefaults.md) | <span data-ttu-id="7bf84-125">无</span><span class="sxs-lookup"><span data-stu-id="7bf84-125">None</span></span> | <span data-ttu-id="7bf84-126">重置打印机的默认设置。</span><span class="sxs-lookup"><span data-stu-id="7bf84-126">Reset a printer's default settings.</span></span> |
| [<span data-ttu-id="7bf84-127">列出作业</span><span class="sxs-lookup"><span data-stu-id="7bf84-127">List jobs</span></span>](../api/printer-list-jobs.md) | <span data-ttu-id="7bf84-128">[printJob](printjob.md)集合</span><span class="sxs-lookup"><span data-stu-id="7bf84-128">[printJob](printjob.md) collection</span></span> | <span data-ttu-id="7bf84-129">获取排队等待打印机处理的打印作业的列表。</span><span class="sxs-lookup"><span data-stu-id="7bf84-129">Get a list of print jobs that are queued for processing by the printer.</span></span> |
| [<span data-ttu-id="7bf84-130">创建作业</span><span class="sxs-lookup"><span data-stu-id="7bf84-130">Create job</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="7bf84-131">printJob</span><span class="sxs-lookup"><span data-stu-id="7bf84-131">printJob</span></span>](printjob.md) | <span data-ttu-id="7bf84-132">为打印机创建一个新的打印作业。</span><span class="sxs-lookup"><span data-stu-id="7bf84-132">Create a new print job for the printer.</span></span> <span data-ttu-id="7bf84-133">若要开始打印作业，请使用[startPrintJob](../api/printjob-startprintjob.md)。</span><span class="sxs-lookup"><span data-stu-id="7bf84-133">To start printing the job, use [startPrintJob](../api/printjob-startprintjob.md).</span></span> |
| [<span data-ttu-id="7bf84-134">列出连接器</span><span class="sxs-lookup"><span data-stu-id="7bf84-134">List connectors</span></span>](../api/printer-list-connectors.md) | <span data-ttu-id="7bf84-135">[printConnector](printconnector.md)集合</span><span class="sxs-lookup"><span data-stu-id="7bf84-135">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="7bf84-136">获取此打印机关联的连接器的列表。</span><span class="sxs-lookup"><span data-stu-id="7bf84-136">Get a list of connectors that this printer is associated with.</span></span> |
| [<span data-ttu-id="7bf84-137">列出 allowedUsers</span><span class="sxs-lookup"><span data-stu-id="7bf84-137">List allowedUsers</span></span>](../api/printer-list-allowedusers.md) | <span data-ttu-id="7bf84-138">[printUserIdentity](printuseridentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="7bf84-138">[printUserIdentity](printuseridentity.md) collection</span></span> | <span data-ttu-id="7bf84-139">检索已授予访问权限以将打印作业提交到关联打印机的用户的列表。</span><span class="sxs-lookup"><span data-stu-id="7bf84-139">Retrieve a list of users who have been granted access to submit print jobs to the associated printer.</span></span> |
| [<span data-ttu-id="7bf84-140">添加 allowedUser</span><span class="sxs-lookup"><span data-stu-id="7bf84-140">Add allowedUser</span></span>](../api/printer-post-allowedusers.md) | <span data-ttu-id="7bf84-141">无</span><span class="sxs-lookup"><span data-stu-id="7bf84-141">None</span></span> | <span data-ttu-id="7bf84-142">向指定的用户授予向关联打印机提交打印作业的权限。</span><span class="sxs-lookup"><span data-stu-id="7bf84-142">Grant the specified user access to submit print jobs to the associated printer.</span></span> |
| [<span data-ttu-id="7bf84-143">删除 allowedUser</span><span class="sxs-lookup"><span data-stu-id="7bf84-143">Remove allowedUser</span></span>](../api/printer-delete-alloweduser.md) | <span data-ttu-id="7bf84-144">无</span><span class="sxs-lookup"><span data-stu-id="7bf84-144">None</span></span> | <span data-ttu-id="7bf84-145">撤销指定用户的打印机访问权限。</span><span class="sxs-lookup"><span data-stu-id="7bf84-145">Revoke printer access from the specified user.</span></span> |
| [<span data-ttu-id="7bf84-146">列出 allowedGroups</span><span class="sxs-lookup"><span data-stu-id="7bf84-146">List allowedGroups</span></span>](../api/printer-list-allowedgroups.md) | <span data-ttu-id="7bf84-147">[printIdentity](printidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="7bf84-147">[printIdentity](printidentity.md) collection</span></span> | <span data-ttu-id="7bf84-148">检索已向其授予将打印作业提交到关联打印机的访问权限的组列表。</span><span class="sxs-lookup"><span data-stu-id="7bf84-148">Retrieve a list of groups which have been granted access to submit print jobs to the associated printer.</span></span> |
| [<span data-ttu-id="7bf84-149">添加 allowedGroup</span><span class="sxs-lookup"><span data-stu-id="7bf84-149">Add allowedGroup</span></span>](../api/printer-post-allowedgroups.md) | <span data-ttu-id="7bf84-150">无</span><span class="sxs-lookup"><span data-stu-id="7bf84-150">None</span></span> | <span data-ttu-id="7bf84-151">向指定的组授予向关联打印机提交打印作业的权限。</span><span class="sxs-lookup"><span data-stu-id="7bf84-151">Grant the specified group access to submit print jobs to the associated printer.</span></span> |
| [<span data-ttu-id="7bf84-152">删除 allowedGroup</span><span class="sxs-lookup"><span data-stu-id="7bf84-152">Remove allowedGroup</span></span>](../api/printer-delete-allowedgroup.md) | <span data-ttu-id="7bf84-153">无</span><span class="sxs-lookup"><span data-stu-id="7bf84-153">None</span></span> | <span data-ttu-id="7bf84-154">撤销指定组的打印机访问权限。</span><span class="sxs-lookup"><span data-stu-id="7bf84-154">Revoke printer access from the specified group.</span></span> |

## <a name="properties"></a><span data-ttu-id="7bf84-155">属性</span><span class="sxs-lookup"><span data-stu-id="7bf84-155">Properties</span></span>
| <span data-ttu-id="7bf84-156">属性</span><span class="sxs-lookup"><span data-stu-id="7bf84-156">Property</span></span>     | <span data-ttu-id="7bf84-157">类型</span><span class="sxs-lookup"><span data-stu-id="7bf84-157">Type</span></span>        | <span data-ttu-id="7bf84-158">说明</span><span class="sxs-lookup"><span data-stu-id="7bf84-158">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7bf84-159">id</span><span class="sxs-lookup"><span data-stu-id="7bf84-159">id</span></span>|<span data-ttu-id="7bf84-160">String</span><span class="sxs-lookup"><span data-stu-id="7bf84-160">String</span></span>|<span data-ttu-id="7bf84-161">文档的标识符。</span><span class="sxs-lookup"><span data-stu-id="7bf84-161">The document's identifier.</span></span> <span data-ttu-id="7bf84-162">只读。</span><span class="sxs-lookup"><span data-stu-id="7bf84-162">Read-only.</span></span>|
|<span data-ttu-id="7bf84-163">displayName</span><span class="sxs-lookup"><span data-stu-id="7bf84-163">displayName</span></span>|<span data-ttu-id="7bf84-164">字符串</span><span class="sxs-lookup"><span data-stu-id="7bf84-164">String</span></span>|<span data-ttu-id="7bf84-165">打印机的名称。</span><span class="sxs-lookup"><span data-stu-id="7bf84-165">The name of the printer.</span></span>|
|<span data-ttu-id="7bf84-166">manufacturer</span><span class="sxs-lookup"><span data-stu-id="7bf84-166">manufacturer</span></span>|<span data-ttu-id="7bf84-167">String</span><span class="sxs-lookup"><span data-stu-id="7bf84-167">String</span></span>|<span data-ttu-id="7bf84-168">打印机报告的制造商。</span><span class="sxs-lookup"><span data-stu-id="7bf84-168">The manufacturer reported by the printer.</span></span> <span data-ttu-id="7bf84-169">只读。</span><span class="sxs-lookup"><span data-stu-id="7bf84-169">Read-only.</span></span>|
|<span data-ttu-id="7bf84-170">model</span><span class="sxs-lookup"><span data-stu-id="7bf84-170">model</span></span>|<span data-ttu-id="7bf84-171">String</span><span class="sxs-lookup"><span data-stu-id="7bf84-171">String</span></span>|<span data-ttu-id="7bf84-172">打印机报告的模型名称。</span><span class="sxs-lookup"><span data-stu-id="7bf84-172">The model name reported by the printer.</span></span> <span data-ttu-id="7bf84-173">只读。</span><span class="sxs-lookup"><span data-stu-id="7bf84-173">Read-only.</span></span>|
|<span data-ttu-id="7bf84-174">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="7bf84-174">registeredDateTime</span></span>|<span data-ttu-id="7bf84-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7bf84-175">DateTimeOffset</span></span>|<span data-ttu-id="7bf84-176">注册打印机时的 DateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="7bf84-176">The DateTimeOffset when the printer was registered.</span></span> <span data-ttu-id="7bf84-177">只读。</span><span class="sxs-lookup"><span data-stu-id="7bf84-177">Read-only.</span></span>|
|<span data-ttu-id="7bf84-178">status</span><span class="sxs-lookup"><span data-stu-id="7bf84-178">status</span></span>|[<span data-ttu-id="7bf84-179">printerStatus</span><span class="sxs-lookup"><span data-stu-id="7bf84-179">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="7bf84-180">打印机的处理状态，包括任何错误。</span><span class="sxs-lookup"><span data-stu-id="7bf84-180">The processing status of the printer, including any errors.</span></span> <span data-ttu-id="7bf84-181">只读。</span><span class="sxs-lookup"><span data-stu-id="7bf84-181">Read-only.</span></span>|
|<span data-ttu-id="7bf84-182">isShared</span><span class="sxs-lookup"><span data-stu-id="7bf84-182">isShared</span></span>|<span data-ttu-id="7bf84-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="7bf84-183">Boolean</span></span>|<span data-ttu-id="7bf84-184">如果打印机是共享的，则为 True;否则为 false。</span><span class="sxs-lookup"><span data-stu-id="7bf84-184">True if the printer is shared; false otherwise.</span></span> <span data-ttu-id="7bf84-185">只读。</span><span class="sxs-lookup"><span data-stu-id="7bf84-185">Read-only.</span></span>|
|<span data-ttu-id="7bf84-186">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="7bf84-186">isAcceptingJobs</span></span>|<span data-ttu-id="7bf84-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="7bf84-187">Boolean</span></span>|<span data-ttu-id="7bf84-188">打印机当前是否正在接受新的打印作业。</span><span class="sxs-lookup"><span data-stu-id="7bf84-188">Whether the printer is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="7bf84-189">位置</span><span class="sxs-lookup"><span data-stu-id="7bf84-189">location</span></span>|[<span data-ttu-id="7bf84-190">printerLocation</span><span class="sxs-lookup"><span data-stu-id="7bf84-190">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="7bf84-191">打印机的物理和/或组织位置。</span><span class="sxs-lookup"><span data-stu-id="7bf84-191">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="7bf84-192">缺省值</span><span class="sxs-lookup"><span data-stu-id="7bf84-192">defaults</span></span>|[<span data-ttu-id="7bf84-193">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="7bf84-193">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="7bf84-194">打印机的默认打印设置。</span><span class="sxs-lookup"><span data-stu-id="7bf84-194">The printer's default print settings.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7bf84-195">关系</span><span class="sxs-lookup"><span data-stu-id="7bf84-195">Relationships</span></span>
| <span data-ttu-id="7bf84-196">关系</span><span class="sxs-lookup"><span data-stu-id="7bf84-196">Relationship</span></span> | <span data-ttu-id="7bf84-197">类型</span><span class="sxs-lookup"><span data-stu-id="7bf84-197">Type</span></span>        | <span data-ttu-id="7bf84-198">说明</span><span class="sxs-lookup"><span data-stu-id="7bf84-198">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7bf84-199">jobs</span><span class="sxs-lookup"><span data-stu-id="7bf84-199">jobs</span></span>|<span data-ttu-id="7bf84-200">[printJob](printjob.md)集合</span><span class="sxs-lookup"><span data-stu-id="7bf84-200">[printJob](printjob.md) collection</span></span>| <span data-ttu-id="7bf84-201">打印机排队等待打印的作业的列表。</span><span class="sxs-lookup"><span data-stu-id="7bf84-201">The list of jobs that are queued for printing by the printer.</span></span>|
|<span data-ttu-id="7bf84-202">shares</span><span class="sxs-lookup"><span data-stu-id="7bf84-202">shares</span></span>|<span data-ttu-id="7bf84-203">[printerShare](printershare.md)集合</span><span class="sxs-lookup"><span data-stu-id="7bf84-203">[printerShare](printershare.md) collection</span></span>| <span data-ttu-id="7bf84-204">与打印机关联的 printerShares 的列表。</span><span class="sxs-lookup"><span data-stu-id="7bf84-204">The list of printerShares that are associated with the printer.</span></span> <span data-ttu-id="7bf84-205">只读。</span><span class="sxs-lookup"><span data-stu-id="7bf84-205">Read-only.</span></span> <span data-ttu-id="7bf84-206">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="7bf84-206">Nullable.</span></span>|
|<span data-ttu-id="7bf84-207">插槽</span><span class="sxs-lookup"><span data-stu-id="7bf84-207">connectors</span></span>|[<span data-ttu-id="7bf84-208">printConnector</span><span class="sxs-lookup"><span data-stu-id="7bf84-208">printConnector</span></span>](printconnector.md)|<span data-ttu-id="7bf84-209">与打印机关联的连接器。</span><span class="sxs-lookup"><span data-stu-id="7bf84-209">The connectors that are associated with the printer.</span></span>|
|<span data-ttu-id="7bf84-210">allowedUsers</span><span class="sxs-lookup"><span data-stu-id="7bf84-210">allowedUsers</span></span>|<span data-ttu-id="7bf84-211">[printUserIdentity](printuseridentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="7bf84-211">[printUserIdentity](printuseridentity.md) collection</span></span>|<span data-ttu-id="7bf84-212">有权使用打印机打印的用户。</span><span class="sxs-lookup"><span data-stu-id="7bf84-212">The users who have access to print using the printer.</span></span>|
|<span data-ttu-id="7bf84-213">allowedGroups</span><span class="sxs-lookup"><span data-stu-id="7bf84-213">allowedGroups</span></span>|[<span data-ttu-id="7bf84-214">printIdentity</span><span class="sxs-lookup"><span data-stu-id="7bf84-214">printIdentity</span></span>](printidentity.md)|<span data-ttu-id="7bf84-215">其用户有权使用打印机打印的组。</span><span class="sxs-lookup"><span data-stu-id="7bf84-215">The groups whose users have access to print using the printer.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7bf84-216">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7bf84-216">JSON representation</span></span>

<span data-ttu-id="7bf84-217">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7bf84-217">The following is a JSON representation of the resource.</span></span>

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