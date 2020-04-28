---
title: 打印机资源类型
description: 表示已向通用打印服务注册的物理打印机设备。 打印机资源可用于管理打印作业、打印机设置、打印机元数据和注册状态。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 6688f36aef36fa8efc00bf2458911ca719f697cc
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917584"
---
# <a name="printer-resource-type"></a><span data-ttu-id="e10b0-104">打印机资源类型</span><span class="sxs-lookup"><span data-stu-id="e10b0-104">printer resource type</span></span>

<span data-ttu-id="e10b0-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e10b0-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e10b0-106">表示已向通用打印服务注册的物理打印机设备。</span><span class="sxs-lookup"><span data-stu-id="e10b0-106">Represents a physical printer device that has been registered with the Universal Print service.</span></span> <span data-ttu-id="e10b0-107">打印机资源可用于管理打印作业、打印机设置、打印机元数据和注册状态。</span><span class="sxs-lookup"><span data-stu-id="e10b0-107">Printer resources can be used to manage print jobs, printer settings, printer metadata and registration status.</span></span>

## <a name="methods"></a><span data-ttu-id="e10b0-108">Methods</span><span class="sxs-lookup"><span data-stu-id="e10b0-108">Methods</span></span>

| <span data-ttu-id="e10b0-109">方法</span><span class="sxs-lookup"><span data-stu-id="e10b0-109">Method</span></span>       | <span data-ttu-id="e10b0-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e10b0-110">Return Type</span></span> | <span data-ttu-id="e10b0-111">说明</span><span class="sxs-lookup"><span data-stu-id="e10b0-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e10b0-112">获取打印机</span><span class="sxs-lookup"><span data-stu-id="e10b0-112">Get printer</span></span>](../api/printer-get.md) | [<span data-ttu-id="e10b0-113">印刷</span><span class="sxs-lookup"><span data-stu-id="e10b0-113">printer</span></span>](printer.md) | <span data-ttu-id="e10b0-114">读取 printer 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e10b0-114">Read the properties and relationships of the printer object.</span></span> |
| [<span data-ttu-id="e10b0-115">更新</span><span class="sxs-lookup"><span data-stu-id="e10b0-115">Update</span></span>](../api/printer-update.md) | [<span data-ttu-id="e10b0-116">印刷</span><span class="sxs-lookup"><span data-stu-id="e10b0-116">printer</span></span>](printer.md) | <span data-ttu-id="e10b0-117">更新 printer 对象。</span><span class="sxs-lookup"><span data-stu-id="e10b0-117">Update the printer object.</span></span> |
| [<span data-ttu-id="e10b0-118">删除</span><span class="sxs-lookup"><span data-stu-id="e10b0-118">Delete</span></span>](../api/printer-delete.md) | <span data-ttu-id="e10b0-119">无</span><span class="sxs-lookup"><span data-stu-id="e10b0-119">None</span></span> | <span data-ttu-id="e10b0-120">在通用打印服务中注销物理 printerfrom。</span><span class="sxs-lookup"><span data-stu-id="e10b0-120">Unregister the physical printerfrom the Universal Print service.</span></span> |
| [<span data-ttu-id="e10b0-121">getCapabilities</span><span class="sxs-lookup"><span data-stu-id="e10b0-121">getCapabilities</span></span>](../api/printer-getcapabilities.md) | [<span data-ttu-id="e10b0-122">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="e10b0-122">printerCapabilities</span></span>](printercapabilities.md) | <span data-ttu-id="e10b0-123">获取打印机的功能列表。</span><span class="sxs-lookup"><span data-stu-id="e10b0-123">Get a list of capabilities for the printer.</span></span> |
| [<span data-ttu-id="e10b0-124">resetDefaults</span><span class="sxs-lookup"><span data-stu-id="e10b0-124">resetDefaults</span></span>](../api/printer-resetdefaults.md) | <span data-ttu-id="e10b0-125">无</span><span class="sxs-lookup"><span data-stu-id="e10b0-125">None</span></span> | <span data-ttu-id="e10b0-126">重置打印机的默认设置。</span><span class="sxs-lookup"><span data-stu-id="e10b0-126">Reset a printer's default settings.</span></span> |
| [<span data-ttu-id="e10b0-127">列出作业</span><span class="sxs-lookup"><span data-stu-id="e10b0-127">List jobs</span></span>](../api/printer-list-jobs.md) | <span data-ttu-id="e10b0-128">[printJob](printjob.md)集合</span><span class="sxs-lookup"><span data-stu-id="e10b0-128">[printJob](printjob.md) collection</span></span> | <span data-ttu-id="e10b0-129">获取排队等待打印机处理的打印作业的列表。</span><span class="sxs-lookup"><span data-stu-id="e10b0-129">Get a list of print jobs that are queued for processing by the printer.</span></span> |
| [<span data-ttu-id="e10b0-130">创建作业</span><span class="sxs-lookup"><span data-stu-id="e10b0-130">Create job</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="e10b0-131">printJob</span><span class="sxs-lookup"><span data-stu-id="e10b0-131">printJob</span></span>](printjob.md) | <span data-ttu-id="e10b0-132">为打印机创建一个新的打印作业。</span><span class="sxs-lookup"><span data-stu-id="e10b0-132">Create a new print job for the printer.</span></span> <span data-ttu-id="e10b0-133">若要开始打印作业，请使用[startPrintJob](../api/printjob-startprintjob.md)。</span><span class="sxs-lookup"><span data-stu-id="e10b0-133">To start printing the job, use [startPrintJob](../api/printjob-startprintjob.md).</span></span> |
| [<span data-ttu-id="e10b0-134">列出连接器</span><span class="sxs-lookup"><span data-stu-id="e10b0-134">List connectors</span></span>](../api/printer-list-connectors.md) | <span data-ttu-id="e10b0-135">[printConnector](printconnector.md)集合</span><span class="sxs-lookup"><span data-stu-id="e10b0-135">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="e10b0-136">获取此打印机关联的连接器的列表。</span><span class="sxs-lookup"><span data-stu-id="e10b0-136">Get a list of connectors that this printer is associated with.</span></span> |
| [<span data-ttu-id="e10b0-137">列出 allowedUsers</span><span class="sxs-lookup"><span data-stu-id="e10b0-137">List allowedUsers</span></span>](../api/printer-list-allowedusers.md) | <span data-ttu-id="e10b0-138">[printUserIdentity](printuseridentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="e10b0-138">[printUserIdentity](printuseridentity.md) collection</span></span> | <span data-ttu-id="e10b0-139">检索已授予访问权限以将打印作业提交到关联打印机的用户的列表。</span><span class="sxs-lookup"><span data-stu-id="e10b0-139">Retrieve a list of users who have been granted access to submit print jobs to the associated printer.</span></span> |
| [<span data-ttu-id="e10b0-140">添加 allowedUser</span><span class="sxs-lookup"><span data-stu-id="e10b0-140">Add allowedUser</span></span>](../api/printer-post-allowedusers.md) | <span data-ttu-id="e10b0-141">无</span><span class="sxs-lookup"><span data-stu-id="e10b0-141">None</span></span> | <span data-ttu-id="e10b0-142">向指定的用户授予向关联打印机提交打印作业的权限。</span><span class="sxs-lookup"><span data-stu-id="e10b0-142">Grant the specified user access to submit print jobs to the associated printer.</span></span> |
| [<span data-ttu-id="e10b0-143">删除 allowedUser</span><span class="sxs-lookup"><span data-stu-id="e10b0-143">Remove allowedUser</span></span>](../api/printer-delete-alloweduser.md) | <span data-ttu-id="e10b0-144">无</span><span class="sxs-lookup"><span data-stu-id="e10b0-144">None</span></span> | <span data-ttu-id="e10b0-145">撤销指定用户的打印机访问权限。</span><span class="sxs-lookup"><span data-stu-id="e10b0-145">Revoke printer access from the specified user.</span></span> |
| [<span data-ttu-id="e10b0-146">列出 allowedGroups</span><span class="sxs-lookup"><span data-stu-id="e10b0-146">List allowedGroups</span></span>](../api/printer-list-allowedgroups.md) | <span data-ttu-id="e10b0-147">[printIdentity](printidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="e10b0-147">[printIdentity](printidentity.md) collection</span></span> | <span data-ttu-id="e10b0-148">检索已向其授予将打印作业提交到关联打印机的访问权限的组列表。</span><span class="sxs-lookup"><span data-stu-id="e10b0-148">Retrieve a list of groups which have been granted access to submit print jobs to the associated printer.</span></span> |
| [<span data-ttu-id="e10b0-149">添加 allowedGroup</span><span class="sxs-lookup"><span data-stu-id="e10b0-149">Add allowedGroup</span></span>](../api/printer-post-allowedgroups.md) | <span data-ttu-id="e10b0-150">无</span><span class="sxs-lookup"><span data-stu-id="e10b0-150">None</span></span> | <span data-ttu-id="e10b0-151">向指定的组授予向关联打印机提交打印作业的权限。</span><span class="sxs-lookup"><span data-stu-id="e10b0-151">Grant the specified group access to submit print jobs to the associated printer.</span></span> |
| [<span data-ttu-id="e10b0-152">删除 allowedGroup</span><span class="sxs-lookup"><span data-stu-id="e10b0-152">Remove allowedGroup</span></span>](../api/printer-delete-allowedgroup.md) | <span data-ttu-id="e10b0-153">无</span><span class="sxs-lookup"><span data-stu-id="e10b0-153">None</span></span> | <span data-ttu-id="e10b0-154">撤销指定组的打印机访问权限。</span><span class="sxs-lookup"><span data-stu-id="e10b0-154">Revoke printer access from the specified group.</span></span> |

## <a name="properties"></a><span data-ttu-id="e10b0-155">属性</span><span class="sxs-lookup"><span data-stu-id="e10b0-155">Properties</span></span>
| <span data-ttu-id="e10b0-156">属性</span><span class="sxs-lookup"><span data-stu-id="e10b0-156">Property</span></span>     | <span data-ttu-id="e10b0-157">类型</span><span class="sxs-lookup"><span data-stu-id="e10b0-157">Type</span></span>        | <span data-ttu-id="e10b0-158">说明</span><span class="sxs-lookup"><span data-stu-id="e10b0-158">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e10b0-159">id</span><span class="sxs-lookup"><span data-stu-id="e10b0-159">id</span></span>|<span data-ttu-id="e10b0-160">String</span><span class="sxs-lookup"><span data-stu-id="e10b0-160">String</span></span>|<span data-ttu-id="e10b0-161">文档的标识符。</span><span class="sxs-lookup"><span data-stu-id="e10b0-161">The document's identifier.</span></span> <span data-ttu-id="e10b0-162">只读。</span><span class="sxs-lookup"><span data-stu-id="e10b0-162">Read-only.</span></span>|
|<span data-ttu-id="e10b0-163">name</span><span class="sxs-lookup"><span data-stu-id="e10b0-163">name</span></span>|<span data-ttu-id="e10b0-164">String</span><span class="sxs-lookup"><span data-stu-id="e10b0-164">String</span></span>|<span data-ttu-id="e10b0-165">打印机的名称。</span><span class="sxs-lookup"><span data-stu-id="e10b0-165">The name of the printer.</span></span>|
|<span data-ttu-id="e10b0-166">manufacturer</span><span class="sxs-lookup"><span data-stu-id="e10b0-166">manufacturer</span></span>|<span data-ttu-id="e10b0-167">String</span><span class="sxs-lookup"><span data-stu-id="e10b0-167">String</span></span>|<span data-ttu-id="e10b0-168">打印机报告的制造商。</span><span class="sxs-lookup"><span data-stu-id="e10b0-168">The manufacturer reported by the printer.</span></span> <span data-ttu-id="e10b0-169">只读。</span><span class="sxs-lookup"><span data-stu-id="e10b0-169">Read-only.</span></span>|
|<span data-ttu-id="e10b0-170">model</span><span class="sxs-lookup"><span data-stu-id="e10b0-170">model</span></span>|<span data-ttu-id="e10b0-171">String</span><span class="sxs-lookup"><span data-stu-id="e10b0-171">String</span></span>|<span data-ttu-id="e10b0-172">打印机报告的模型名称。</span><span class="sxs-lookup"><span data-stu-id="e10b0-172">The model name reported by the printer.</span></span> <span data-ttu-id="e10b0-173">只读。</span><span class="sxs-lookup"><span data-stu-id="e10b0-173">Read-only.</span></span>|
|<span data-ttu-id="e10b0-174">registeredBy</span><span class="sxs-lookup"><span data-stu-id="e10b0-174">registeredBy</span></span>|[<span data-ttu-id="e10b0-175">printUserIdentity</span><span class="sxs-lookup"><span data-stu-id="e10b0-175">printUserIdentity</span></span>](printuseridentity.md)|<span data-ttu-id="e10b0-176">注册打印机的用户。</span><span class="sxs-lookup"><span data-stu-id="e10b0-176">The user who registered the printer.</span></span>|
|<span data-ttu-id="e10b0-177">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="e10b0-177">registeredDateTime</span></span>|<span data-ttu-id="e10b0-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e10b0-178">DateTimeOffset</span></span>|<span data-ttu-id="e10b0-179">注册打印机时的 DateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="e10b0-179">The DateTimeOffset when the printer was registered.</span></span> <span data-ttu-id="e10b0-180">只读。</span><span class="sxs-lookup"><span data-stu-id="e10b0-180">Read-only.</span></span>|
|<span data-ttu-id="e10b0-181">状态</span><span class="sxs-lookup"><span data-stu-id="e10b0-181">status</span></span>|[<span data-ttu-id="e10b0-182">printerStatus</span><span class="sxs-lookup"><span data-stu-id="e10b0-182">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="e10b0-183">打印机的处理状态，包括任何错误。</span><span class="sxs-lookup"><span data-stu-id="e10b0-183">The processing status of the printer, including any errors.</span></span> <span data-ttu-id="e10b0-184">只读。</span><span class="sxs-lookup"><span data-stu-id="e10b0-184">Read-only.</span></span>|
|<span data-ttu-id="e10b0-185">isShared</span><span class="sxs-lookup"><span data-stu-id="e10b0-185">isShared</span></span>|<span data-ttu-id="e10b0-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="e10b0-186">Boolean</span></span>|<span data-ttu-id="e10b0-187">如果打印机是共享的，则为 True;否则为 false。</span><span class="sxs-lookup"><span data-stu-id="e10b0-187">True if the printer is shared; false otherwise.</span></span> <span data-ttu-id="e10b0-188">只读。</span><span class="sxs-lookup"><span data-stu-id="e10b0-188">Read-only.</span></span>|
|<span data-ttu-id="e10b0-189">acceptingJobs</span><span class="sxs-lookup"><span data-stu-id="e10b0-189">acceptingJobs</span></span>|<span data-ttu-id="e10b0-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="e10b0-190">Boolean</span></span>|<span data-ttu-id="e10b0-191">打印机当前是否正在接受新的打印作业。</span><span class="sxs-lookup"><span data-stu-id="e10b0-191">Whether the printer is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="e10b0-192">位置</span><span class="sxs-lookup"><span data-stu-id="e10b0-192">location</span></span>|[<span data-ttu-id="e10b0-193">printerLocation</span><span class="sxs-lookup"><span data-stu-id="e10b0-193">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="e10b0-194">打印机的物理和/或组织位置。</span><span class="sxs-lookup"><span data-stu-id="e10b0-194">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="e10b0-195">缺省值</span><span class="sxs-lookup"><span data-stu-id="e10b0-195">defaults</span></span>|[<span data-ttu-id="e10b0-196">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="e10b0-196">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="e10b0-197">打印机的默认打印设置。</span><span class="sxs-lookup"><span data-stu-id="e10b0-197">The printer's default print settings.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e10b0-198">关系</span><span class="sxs-lookup"><span data-stu-id="e10b0-198">Relationships</span></span>
| <span data-ttu-id="e10b0-199">关系</span><span class="sxs-lookup"><span data-stu-id="e10b0-199">Relationship</span></span> | <span data-ttu-id="e10b0-200">类型</span><span class="sxs-lookup"><span data-stu-id="e10b0-200">Type</span></span>        | <span data-ttu-id="e10b0-201">说明</span><span class="sxs-lookup"><span data-stu-id="e10b0-201">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e10b0-202">jobs</span><span class="sxs-lookup"><span data-stu-id="e10b0-202">jobs</span></span>|<span data-ttu-id="e10b0-203">[printJob](printjob.md)集合</span><span class="sxs-lookup"><span data-stu-id="e10b0-203">[printJob](printjob.md) collection</span></span>| <span data-ttu-id="e10b0-204">打印机排队等待打印的作业的列表。</span><span class="sxs-lookup"><span data-stu-id="e10b0-204">The list of jobs that are queued for printing by the printer.</span></span> <span data-ttu-id="e10b0-205">只读。</span><span class="sxs-lookup"><span data-stu-id="e10b0-205">Read-only.</span></span> <span data-ttu-id="e10b0-206">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="e10b0-206">Nullable.</span></span>|
|<span data-ttu-id="e10b0-207">shares</span><span class="sxs-lookup"><span data-stu-id="e10b0-207">shares</span></span>|[<span data-ttu-id="e10b0-208">printerShare</span><span class="sxs-lookup"><span data-stu-id="e10b0-208">printerShare</span></span>](printershare.md)| <span data-ttu-id="e10b0-209">与打印机关联的 printerShare。</span><span class="sxs-lookup"><span data-stu-id="e10b0-209">The printerShare that is associated with the printer.</span></span> <span data-ttu-id="e10b0-210">只读。</span><span class="sxs-lookup"><span data-stu-id="e10b0-210">Read-only.</span></span> <span data-ttu-id="e10b0-211">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="e10b0-211">Nullable.</span></span>|
|<span data-ttu-id="e10b0-212">插槽</span><span class="sxs-lookup"><span data-stu-id="e10b0-212">connectors</span></span>|[<span data-ttu-id="e10b0-213">printConnector</span><span class="sxs-lookup"><span data-stu-id="e10b0-213">printConnector</span></span>](printconnector.md)|<span data-ttu-id="e10b0-214">与打印机关联的连接器。</span><span class="sxs-lookup"><span data-stu-id="e10b0-214">The connectors that are associated with the printer.</span></span>|
|<span data-ttu-id="e10b0-215">allowedUsers</span><span class="sxs-lookup"><span data-stu-id="e10b0-215">allowedUsers</span></span>|<span data-ttu-id="e10b0-216">[printUserIdentity](printuseridentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="e10b0-216">[printUserIdentity](printuseridentity.md) collection</span></span>|<span data-ttu-id="e10b0-217">有权使用打印机打印的用户。</span><span class="sxs-lookup"><span data-stu-id="e10b0-217">The users who have access to print using the printer.</span></span>|
|<span data-ttu-id="e10b0-218">allowedGroups</span><span class="sxs-lookup"><span data-stu-id="e10b0-218">allowedGroups</span></span>|[<span data-ttu-id="e10b0-219">printIdentity</span><span class="sxs-lookup"><span data-stu-id="e10b0-219">printIdentity</span></span>](printidentity.md)|<span data-ttu-id="e10b0-220">其用户有权使用打印机打印的组。</span><span class="sxs-lookup"><span data-stu-id="e10b0-220">The groups whose users have access to print using the printer.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e10b0-221">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e10b0-221">JSON representation</span></span>

<span data-ttu-id="e10b0-222">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e10b0-222">The following is a JSON representation of the resource.</span></span>

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