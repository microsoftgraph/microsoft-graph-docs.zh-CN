---
title: printerShare 资源类型
description: 表示可供用户和打印应用程序发现的打印机。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 4fc729a41105340cc4066ee238c8d1ace3490765
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848225"
---
# <a name="printershare-resource-type"></a><span data-ttu-id="4a912-103">printerShare 资源类型</span><span class="sxs-lookup"><span data-stu-id="4a912-103">printerShare resource type</span></span>

<span data-ttu-id="4a912-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a912-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a912-105">表示可供用户和打印应用程序发现的打印机。</span><span class="sxs-lookup"><span data-stu-id="4a912-105">Represents a printer that is intended to be discoverable by users and printing applications.</span></span>

## <a name="methods"></a><span data-ttu-id="4a912-106">方法</span><span class="sxs-lookup"><span data-stu-id="4a912-106">Methods</span></span>

| <span data-ttu-id="4a912-107">方法</span><span class="sxs-lookup"><span data-stu-id="4a912-107">Method</span></span>       | <span data-ttu-id="4a912-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="4a912-108">Return Type</span></span> | <span data-ttu-id="4a912-109">Description</span><span class="sxs-lookup"><span data-stu-id="4a912-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4a912-110">List</span><span class="sxs-lookup"><span data-stu-id="4a912-110">List</span></span>](../api/print-list-shares.md) | <span data-ttu-id="4a912-111">[printerShare](printershare.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4a912-111">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="4a912-112">获取租户中的打印机共享的列表。</span><span class="sxs-lookup"><span data-stu-id="4a912-112">Get a list of printer shares in the tenant.</span></span> |
| [<span data-ttu-id="4a912-113">获取</span><span class="sxs-lookup"><span data-stu-id="4a912-113">Get</span></span>](../api/printershare-get.md) | [<span data-ttu-id="4a912-114">printerShare</span><span class="sxs-lookup"><span data-stu-id="4a912-114">printerShare</span></span>](printershare.md) | <span data-ttu-id="4a912-115">读取 **printerShare** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4a912-115">Read properties and relationships of a **printerShare** object.</span></span> |
| [<span data-ttu-id="4a912-116">更新</span><span class="sxs-lookup"><span data-stu-id="4a912-116">Update</span></span>](../api/printershare-update.md) | [<span data-ttu-id="4a912-117">printerShare</span><span class="sxs-lookup"><span data-stu-id="4a912-117">printerShare</span></span>](printershare.md) | <span data-ttu-id="4a912-118">更新 **printerShare** 对象。</span><span class="sxs-lookup"><span data-stu-id="4a912-118">Update a **printerShare** object.</span></span> |
| [<span data-ttu-id="4a912-119">删除</span><span class="sxs-lookup"><span data-stu-id="4a912-119">Delete</span></span>](../api/printershare-delete.md) | <span data-ttu-id="4a912-120">无</span><span class="sxs-lookup"><span data-stu-id="4a912-120">None</span></span> | <span data-ttu-id="4a912-121">取消打印机的共享。</span><span class="sxs-lookup"><span data-stu-id="4a912-121">Unshare a printer.</span></span> |
| [<span data-ttu-id="4a912-122">列出作业</span><span class="sxs-lookup"><span data-stu-id="4a912-122">List jobs</span></span>](../api/printershare-list-jobs.md) | <span data-ttu-id="4a912-123">[printJob](printjob.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4a912-123">[printJob](printjob.md) collection</span></span> | <span data-ttu-id="4a912-124">获取排队等待处理的打印作业的列表 printerShare。</span><span class="sxs-lookup"><span data-stu-id="4a912-124">Get a list of print jobs that are queued for processing by the printerShare.</span></span> |
| [<span data-ttu-id="4a912-125">创建作业</span><span class="sxs-lookup"><span data-stu-id="4a912-125">Create job</span></span>](../api/printershare-post-jobs.md) | [<span data-ttu-id="4a912-126">printJob</span><span class="sxs-lookup"><span data-stu-id="4a912-126">printJob</span></span>](printjob.md) | <span data-ttu-id="4a912-127">为 printerShare 创建新的打印作业。</span><span class="sxs-lookup"><span data-stu-id="4a912-127">Create a new print job for the printerShare.</span></span> <span data-ttu-id="4a912-128">若要开始打印作业，请使用 [start](../api/printjob-start.md)。</span><span class="sxs-lookup"><span data-stu-id="4a912-128">To start printing the job, use [start](../api/printjob-start.md).</span></span> |
| [<span data-ttu-id="4a912-129">列出 allowedUsers</span><span class="sxs-lookup"><span data-stu-id="4a912-129">List allowedUsers</span></span>](../api/printershare-list-allowedusers.md) | <span data-ttu-id="4a912-130">[printUserIdentity](printuseridentity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4a912-130">[printUserIdentity](printuseridentity.md) collection</span></span> | <span data-ttu-id="4a912-131">检索已授予访问权限以将打印作业提交到关联的打印机共享的用户列表。</span><span class="sxs-lookup"><span data-stu-id="4a912-131">Retrieve a list of users who have been granted access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="4a912-132">添加 allowedUser</span><span class="sxs-lookup"><span data-stu-id="4a912-132">Add allowedUser</span></span>](../api/printershare-post-allowedusers.md) | <span data-ttu-id="4a912-133">无</span><span class="sxs-lookup"><span data-stu-id="4a912-133">None</span></span> | <span data-ttu-id="4a912-134">向指定的用户授予将打印作业提交到关联的打印机共享的权限。</span><span class="sxs-lookup"><span data-stu-id="4a912-134">Grant the specified user access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="4a912-135">删除 allowedUser</span><span class="sxs-lookup"><span data-stu-id="4a912-135">Remove allowedUser</span></span>](../api/printershare-delete-alloweduser.md) | <span data-ttu-id="4a912-136">无</span><span class="sxs-lookup"><span data-stu-id="4a912-136">None</span></span> | <span data-ttu-id="4a912-137">撤销指定用户的打印机共享访问权限。</span><span class="sxs-lookup"><span data-stu-id="4a912-137">Revoke printer share access from the specified user.</span></span> |
| [<span data-ttu-id="4a912-138">列出 allowedGroups</span><span class="sxs-lookup"><span data-stu-id="4a912-138">List allowedGroups</span></span>](../api/printershare-list-allowedgroups.md) | <span data-ttu-id="4a912-139">[printIdentity](printidentity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4a912-139">[printIdentity](printidentity.md) collection</span></span> | <span data-ttu-id="4a912-140">检索已授予访问权限的组列表，以将打印作业提交到关联的打印机共享。</span><span class="sxs-lookup"><span data-stu-id="4a912-140">Retrieve a list of groups that have been granted access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="4a912-141">添加 allowedGroup</span><span class="sxs-lookup"><span data-stu-id="4a912-141">Add allowedGroup</span></span>](../api/printershare-post-allowedgroups.md) | <span data-ttu-id="4a912-142">无</span><span class="sxs-lookup"><span data-stu-id="4a912-142">None</span></span> | <span data-ttu-id="4a912-143">向指定的组授予将打印作业提交到关联的打印机共享的权限。</span><span class="sxs-lookup"><span data-stu-id="4a912-143">Grant the specified group access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="4a912-144">删除 allowedGroup</span><span class="sxs-lookup"><span data-stu-id="4a912-144">Remove allowedGroup</span></span>](../api/printershare-delete-allowedgroup.md) | <span data-ttu-id="4a912-145">无</span><span class="sxs-lookup"><span data-stu-id="4a912-145">None</span></span> | <span data-ttu-id="4a912-146">撤销指定组的打印机共享访问权限。</span><span class="sxs-lookup"><span data-stu-id="4a912-146">Revoke printer share access from the specified group.</span></span> |

## <a name="properties"></a><span data-ttu-id="4a912-147">属性</span><span class="sxs-lookup"><span data-stu-id="4a912-147">Properties</span></span>
| <span data-ttu-id="4a912-148">属性</span><span class="sxs-lookup"><span data-stu-id="4a912-148">Property</span></span>     | <span data-ttu-id="4a912-149">类型</span><span class="sxs-lookup"><span data-stu-id="4a912-149">Type</span></span>        | <span data-ttu-id="4a912-150">说明</span><span class="sxs-lookup"><span data-stu-id="4a912-150">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4a912-151">id</span><span class="sxs-lookup"><span data-stu-id="4a912-151">id</span></span>|<span data-ttu-id="4a912-152">String</span><span class="sxs-lookup"><span data-stu-id="4a912-152">String</span></span>| <span data-ttu-id="4a912-153">PrinterShare 的标识符。</span><span class="sxs-lookup"><span data-stu-id="4a912-153">The printerShare's identifier.</span></span> <span data-ttu-id="4a912-154">只读。</span><span class="sxs-lookup"><span data-stu-id="4a912-154">Read-only.</span></span>|
|<span data-ttu-id="4a912-155">displayName</span><span class="sxs-lookup"><span data-stu-id="4a912-155">displayName</span></span>|<span data-ttu-id="4a912-156">String</span><span class="sxs-lookup"><span data-stu-id="4a912-156">String</span></span>|<span data-ttu-id="4a912-157">打印客户端应显示的打印机共享的名称。</span><span class="sxs-lookup"><span data-stu-id="4a912-157">The name of the printer share that print clients should display.</span></span>|
|<span data-ttu-id="4a912-158">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4a912-158">createdDateTime</span></span>|<span data-ttu-id="4a912-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a912-159">DateTimeOffset</span></span>|<span data-ttu-id="4a912-160">创建打印机共享时的 DateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="4a912-160">The DateTimeOffset when the printer share was created.</span></span> <span data-ttu-id="4a912-161">只读。</span><span class="sxs-lookup"><span data-stu-id="4a912-161">Read-only.</span></span>|
|<span data-ttu-id="4a912-162">manufacturer</span><span class="sxs-lookup"><span data-stu-id="4a912-162">manufacturer</span></span>|<span data-ttu-id="4a912-163">String</span><span class="sxs-lookup"><span data-stu-id="4a912-163">String</span></span>|<span data-ttu-id="4a912-164">与此打印机共享关联的打印机报告的制造商。</span><span class="sxs-lookup"><span data-stu-id="4a912-164">The manufacturer reported by the printer associated with this printer share.</span></span> <span data-ttu-id="4a912-165">只读。</span><span class="sxs-lookup"><span data-stu-id="4a912-165">Read-only.</span></span>|
|<span data-ttu-id="4a912-166">model</span><span class="sxs-lookup"><span data-stu-id="4a912-166">model</span></span>|<span data-ttu-id="4a912-167">String</span><span class="sxs-lookup"><span data-stu-id="4a912-167">String</span></span>|<span data-ttu-id="4a912-168">与此打印机共享关联的打印机报告的模型名称。</span><span class="sxs-lookup"><span data-stu-id="4a912-168">The model name reported by the printer associated with this printer share.</span></span> <span data-ttu-id="4a912-169">只读。</span><span class="sxs-lookup"><span data-stu-id="4a912-169">Read-only.</span></span>|
|<span data-ttu-id="4a912-170">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="4a912-170">isAcceptingJobs</span></span>|<span data-ttu-id="4a912-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a912-171">Boolean</span></span>|<span data-ttu-id="4a912-172">与此打印机共享关联的打印机当前是否正在接受新的打印作业。</span><span class="sxs-lookup"><span data-stu-id="4a912-172">Whether the printer associated with this printer share is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="4a912-173">defaults</span><span class="sxs-lookup"><span data-stu-id="4a912-173">defaults</span></span>|[<span data-ttu-id="4a912-174">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="4a912-174">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="4a912-175">与此打印机共享关联的打印机的默认打印设置。</span><span class="sxs-lookup"><span data-stu-id="4a912-175">The default print settings of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="4a912-176">capabilities</span><span class="sxs-lookup"><span data-stu-id="4a912-176">capabilities</span></span>|[<span data-ttu-id="4a912-177">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="4a912-177">printerCapabilities</span></span>](printercapabilities.md)|<span data-ttu-id="4a912-178">与此打印机共享相关联的打印机的功能。</span><span class="sxs-lookup"><span data-stu-id="4a912-178">The capabilities of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="4a912-179">位置</span><span class="sxs-lookup"><span data-stu-id="4a912-179">location</span></span>|[<span data-ttu-id="4a912-180">printerLocation</span><span class="sxs-lookup"><span data-stu-id="4a912-180">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="4a912-181">与此打印机共享关联的打印机的物理和/或组织位置。</span><span class="sxs-lookup"><span data-stu-id="4a912-181">The physical and/or organizational location of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="4a912-182">status</span><span class="sxs-lookup"><span data-stu-id="4a912-182">status</span></span>|[<span data-ttu-id="4a912-183">printerStatus</span><span class="sxs-lookup"><span data-stu-id="4a912-183">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="4a912-184">与此打印机共享关联的打印机的处理状态，包括任何错误。</span><span class="sxs-lookup"><span data-stu-id="4a912-184">The processing status, including any errors, of the printer associated with this printer share.</span></span> <span data-ttu-id="4a912-185">只读。</span><span class="sxs-lookup"><span data-stu-id="4a912-185">Read-only.</span></span>|
|<span data-ttu-id="4a912-186">allowAllUsers</span><span class="sxs-lookup"><span data-stu-id="4a912-186">allowAllUsers</span></span>|<span data-ttu-id="4a912-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a912-187">Boolean</span></span>|<span data-ttu-id="4a912-188">如果为 true，则所有用户和组都将被授予对此打印机共享的访问权限。</span><span class="sxs-lookup"><span data-stu-id="4a912-188">If true, all users and groups will be granted access to this printer share.</span></span> <span data-ttu-id="4a912-189">这将取代由 **allowedUsers** 和 **allowedGroups** 导航属性定义的允许列表。</span><span class="sxs-lookup"><span data-stu-id="4a912-189">This supersedes the allow lists defined by the **allowedUsers** and **allowedGroups** navigation properties.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a912-190">关系</span><span class="sxs-lookup"><span data-stu-id="4a912-190">Relationships</span></span>
| <span data-ttu-id="4a912-191">关系</span><span class="sxs-lookup"><span data-stu-id="4a912-191">Relationship</span></span> | <span data-ttu-id="4a912-192">类型</span><span class="sxs-lookup"><span data-stu-id="4a912-192">Type</span></span>        | <span data-ttu-id="4a912-193">说明</span><span class="sxs-lookup"><span data-stu-id="4a912-193">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4a912-194">印刷</span><span class="sxs-lookup"><span data-stu-id="4a912-194">printer</span></span>|[<span data-ttu-id="4a912-195">印刷</span><span class="sxs-lookup"><span data-stu-id="4a912-195">printer</span></span>](printer.md)|<span data-ttu-id="4a912-196">与此打印机共享相关联的打印机。</span><span class="sxs-lookup"><span data-stu-id="4a912-196">The printer that this printer share is related to.</span></span> |
|<span data-ttu-id="4a912-197">allowedUsers</span><span class="sxs-lookup"><span data-stu-id="4a912-197">allowedUsers</span></span>|<span data-ttu-id="4a912-198">[printUserIdentity](printuseridentity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4a912-198">[printUserIdentity](printuseridentity.md) collection</span></span>|<span data-ttu-id="4a912-199">有权使用打印机打印的用户。</span><span class="sxs-lookup"><span data-stu-id="4a912-199">The users who have access to print using the printer.</span></span>|
|<span data-ttu-id="4a912-200">allowedGroups</span><span class="sxs-lookup"><span data-stu-id="4a912-200">allowedGroups</span></span>|[<span data-ttu-id="4a912-201">printIdentity</span><span class="sxs-lookup"><span data-stu-id="4a912-201">printIdentity</span></span>](printidentity.md)|<span data-ttu-id="4a912-202">其用户有权使用打印机打印的组。</span><span class="sxs-lookup"><span data-stu-id="4a912-202">The groups whose users have access to print using the printer.</span></span>|
|<span data-ttu-id="4a912-203">jobs</span><span class="sxs-lookup"><span data-stu-id="4a912-203">jobs</span></span>|<span data-ttu-id="4a912-204">[printJob](printjob.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4a912-204">[printJob](printjob.md) collection</span></span>| <span data-ttu-id="4a912-205">与此打印机共享关联的打印机排队等待打印的作业列表。</span><span class="sxs-lookup"><span data-stu-id="4a912-205">The list of jobs that are queued for printing by the printer associated with this printer share.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4a912-206">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4a912-206">JSON representation</span></span>

<span data-ttu-id="4a912-207">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a912-207">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerShare",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "manufacturer": "String",
  "model": "String",
  "createdDateTime": "String (timestamp)",
  "isAcceptingJobs": true,
  "allowAllUsers": false,
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
  "description": "printerShare resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


