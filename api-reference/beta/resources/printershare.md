---
title: printerShare 资源类型
description: 表示可供用户和打印应用程序发现的打印机。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 4abfc143c90530fd75965e75044248e79e325483
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731454"
---
# <a name="printershare-resource-type"></a><span data-ttu-id="913f2-103">printerShare 资源类型</span><span class="sxs-lookup"><span data-stu-id="913f2-103">printerShare resource type</span></span>

<span data-ttu-id="913f2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="913f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="913f2-105">表示可供用户和打印应用程序发现的打印机。</span><span class="sxs-lookup"><span data-stu-id="913f2-105">Represents a printer that is intended to be discoverable by users and printing applications.</span></span>

## <a name="methods"></a><span data-ttu-id="913f2-106">Methods</span><span class="sxs-lookup"><span data-stu-id="913f2-106">Methods</span></span>

| <span data-ttu-id="913f2-107">方法</span><span class="sxs-lookup"><span data-stu-id="913f2-107">Method</span></span>       | <span data-ttu-id="913f2-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="913f2-108">Return Type</span></span> | <span data-ttu-id="913f2-109">Description</span><span class="sxs-lookup"><span data-stu-id="913f2-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="913f2-110">List</span><span class="sxs-lookup"><span data-stu-id="913f2-110">List</span></span>](../api/print-list-shares.md) | <span data-ttu-id="913f2-111">[printerShare](printershare.md) 集合</span><span class="sxs-lookup"><span data-stu-id="913f2-111">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="913f2-112">获取租户中的打印机共享的列表。</span><span class="sxs-lookup"><span data-stu-id="913f2-112">Get a list of printer shares in the tenant.</span></span> |
| [<span data-ttu-id="913f2-113">获取</span><span class="sxs-lookup"><span data-stu-id="913f2-113">Get</span></span>](../api/printershare-get.md) | [<span data-ttu-id="913f2-114">printerShare</span><span class="sxs-lookup"><span data-stu-id="913f2-114">printerShare</span></span>](printershare.md) | <span data-ttu-id="913f2-115">读取 **printerShare** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="913f2-115">Read properties and relationships of a **printerShare** object.</span></span> |
| [<span data-ttu-id="913f2-116">更新</span><span class="sxs-lookup"><span data-stu-id="913f2-116">Update</span></span>](../api/printershare-update.md) | [<span data-ttu-id="913f2-117">printerShare</span><span class="sxs-lookup"><span data-stu-id="913f2-117">printerShare</span></span>](printershare.md) | <span data-ttu-id="913f2-118">更新 **printerShare** 对象。</span><span class="sxs-lookup"><span data-stu-id="913f2-118">Update a **printerShare** object.</span></span> |
| [<span data-ttu-id="913f2-119">删除</span><span class="sxs-lookup"><span data-stu-id="913f2-119">Delete</span></span>](../api/printershare-delete.md) | <span data-ttu-id="913f2-120">无</span><span class="sxs-lookup"><span data-stu-id="913f2-120">None</span></span> | <span data-ttu-id="913f2-121">取消打印机的共享。</span><span class="sxs-lookup"><span data-stu-id="913f2-121">Unshare a printer.</span></span> |
| [<span data-ttu-id="913f2-122">列出作业</span><span class="sxs-lookup"><span data-stu-id="913f2-122">List jobs</span></span>](../api/printershare-list-jobs.md) | <span data-ttu-id="913f2-123">[printJob](printjob.md) 集合</span><span class="sxs-lookup"><span data-stu-id="913f2-123">[printJob](printjob.md) collection</span></span> | <span data-ttu-id="913f2-124">获取排队等待处理的打印作业的列表 printerShare。</span><span class="sxs-lookup"><span data-stu-id="913f2-124">Get a list of print jobs that are queued for processing by the printerShare.</span></span> |
| [<span data-ttu-id="913f2-125">创建作业</span><span class="sxs-lookup"><span data-stu-id="913f2-125">Create job</span></span>](../api/printershare-post-jobs.md) | [<span data-ttu-id="913f2-126">printJob</span><span class="sxs-lookup"><span data-stu-id="913f2-126">printJob</span></span>](printjob.md) | <span data-ttu-id="913f2-127">为 printerShare 创建新的打印作业。</span><span class="sxs-lookup"><span data-stu-id="913f2-127">Create a new print job for the printerShare.</span></span> <span data-ttu-id="913f2-128">若要开始打印作业，请使用 [start](../api/printjob-start.md)。</span><span class="sxs-lookup"><span data-stu-id="913f2-128">To start printing the job, use [start](../api/printjob-start.md).</span></span> |
| [<span data-ttu-id="913f2-129">列出 allowedUsers</span><span class="sxs-lookup"><span data-stu-id="913f2-129">List allowedUsers</span></span>](../api/printershare-list-allowedusers.md) | <span data-ttu-id="913f2-130">[printUserIdentity](printuseridentity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="913f2-130">[printUserIdentity](printuseridentity.md) collection</span></span> | <span data-ttu-id="913f2-131">检索已授予访问权限以将打印作业提交到关联的打印机共享的用户列表。</span><span class="sxs-lookup"><span data-stu-id="913f2-131">Retrieve a list of users who have been granted access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="913f2-132">添加 allowedUser</span><span class="sxs-lookup"><span data-stu-id="913f2-132">Add allowedUser</span></span>](../api/printershare-post-allowedusers.md) | <span data-ttu-id="913f2-133">无</span><span class="sxs-lookup"><span data-stu-id="913f2-133">None</span></span> | <span data-ttu-id="913f2-134">向指定的用户授予将打印作业提交到关联的打印机共享的权限。</span><span class="sxs-lookup"><span data-stu-id="913f2-134">Grant the specified user access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="913f2-135">删除 allowedUser</span><span class="sxs-lookup"><span data-stu-id="913f2-135">Remove allowedUser</span></span>](../api/printershare-delete-alloweduser.md) | <span data-ttu-id="913f2-136">无</span><span class="sxs-lookup"><span data-stu-id="913f2-136">None</span></span> | <span data-ttu-id="913f2-137">撤销指定用户的打印机共享访问权限。</span><span class="sxs-lookup"><span data-stu-id="913f2-137">Revoke printer share access from the specified user.</span></span> |
| [<span data-ttu-id="913f2-138">列出 allowedGroups</span><span class="sxs-lookup"><span data-stu-id="913f2-138">List allowedGroups</span></span>](../api/printershare-list-allowedgroups.md) | <span data-ttu-id="913f2-139">[printIdentity](printidentity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="913f2-139">[printIdentity](printidentity.md) collection</span></span> | <span data-ttu-id="913f2-140">检索已授予访问权限的组列表，以将打印作业提交到关联的打印机共享。</span><span class="sxs-lookup"><span data-stu-id="913f2-140">Retrieve a list of groups that have been granted access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="913f2-141">添加 allowedGroup</span><span class="sxs-lookup"><span data-stu-id="913f2-141">Add allowedGroup</span></span>](../api/printershare-post-allowedgroups.md) | <span data-ttu-id="913f2-142">无</span><span class="sxs-lookup"><span data-stu-id="913f2-142">None</span></span> | <span data-ttu-id="913f2-143">向指定的组授予将打印作业提交到关联的打印机共享的权限。</span><span class="sxs-lookup"><span data-stu-id="913f2-143">Grant the specified group access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="913f2-144">删除 allowedGroup</span><span class="sxs-lookup"><span data-stu-id="913f2-144">Remove allowedGroup</span></span>](../api/printershare-delete-allowedgroup.md) | <span data-ttu-id="913f2-145">无</span><span class="sxs-lookup"><span data-stu-id="913f2-145">None</span></span> | <span data-ttu-id="913f2-146">撤销指定组的打印机共享访问权限。</span><span class="sxs-lookup"><span data-stu-id="913f2-146">Revoke printer share access from the specified group.</span></span> |

## <a name="properties"></a><span data-ttu-id="913f2-147">属性</span><span class="sxs-lookup"><span data-stu-id="913f2-147">Properties</span></span>
| <span data-ttu-id="913f2-148">属性</span><span class="sxs-lookup"><span data-stu-id="913f2-148">Property</span></span>     | <span data-ttu-id="913f2-149">类型</span><span class="sxs-lookup"><span data-stu-id="913f2-149">Type</span></span>        | <span data-ttu-id="913f2-150">说明</span><span class="sxs-lookup"><span data-stu-id="913f2-150">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="913f2-151">id</span><span class="sxs-lookup"><span data-stu-id="913f2-151">id</span></span>|<span data-ttu-id="913f2-152">String</span><span class="sxs-lookup"><span data-stu-id="913f2-152">String</span></span>| <span data-ttu-id="913f2-153">PrinterShare 的标识符。</span><span class="sxs-lookup"><span data-stu-id="913f2-153">The printerShare's identifier.</span></span> <span data-ttu-id="913f2-154">只读。</span><span class="sxs-lookup"><span data-stu-id="913f2-154">Read-only.</span></span>|
|<span data-ttu-id="913f2-155">displayName</span><span class="sxs-lookup"><span data-stu-id="913f2-155">displayName</span></span>|<span data-ttu-id="913f2-156">String</span><span class="sxs-lookup"><span data-stu-id="913f2-156">String</span></span>|<span data-ttu-id="913f2-157">打印客户端应显示的打印机共享的名称。</span><span class="sxs-lookup"><span data-stu-id="913f2-157">The name of the printer share that print clients should display.</span></span>|
|<span data-ttu-id="913f2-158">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="913f2-158">createdDateTime</span></span>|<span data-ttu-id="913f2-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="913f2-159">DateTimeOffset</span></span>|<span data-ttu-id="913f2-160">创建打印机共享时的 DateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="913f2-160">The DateTimeOffset when the printer share was created.</span></span> <span data-ttu-id="913f2-161">只读。</span><span class="sxs-lookup"><span data-stu-id="913f2-161">Read-only.</span></span>|
|<span data-ttu-id="913f2-162">manufacturer</span><span class="sxs-lookup"><span data-stu-id="913f2-162">manufacturer</span></span>|<span data-ttu-id="913f2-163">String</span><span class="sxs-lookup"><span data-stu-id="913f2-163">String</span></span>|<span data-ttu-id="913f2-164">与此打印机共享关联的打印机报告的制造商。</span><span class="sxs-lookup"><span data-stu-id="913f2-164">The manufacturer reported by the printer associated with this printer share.</span></span> <span data-ttu-id="913f2-165">只读。</span><span class="sxs-lookup"><span data-stu-id="913f2-165">Read-only.</span></span>|
|<span data-ttu-id="913f2-166">model</span><span class="sxs-lookup"><span data-stu-id="913f2-166">model</span></span>|<span data-ttu-id="913f2-167">String</span><span class="sxs-lookup"><span data-stu-id="913f2-167">String</span></span>|<span data-ttu-id="913f2-168">与此打印机共享关联的打印机报告的模型名称。</span><span class="sxs-lookup"><span data-stu-id="913f2-168">The model name reported by the printer associated with this printer share.</span></span> <span data-ttu-id="913f2-169">只读。</span><span class="sxs-lookup"><span data-stu-id="913f2-169">Read-only.</span></span>|
|<span data-ttu-id="913f2-170">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="913f2-170">isAcceptingJobs</span></span>|<span data-ttu-id="913f2-171">布尔</span><span class="sxs-lookup"><span data-stu-id="913f2-171">Boolean</span></span>|<span data-ttu-id="913f2-172">与此打印机共享关联的打印机当前是否正在接受新的打印作业。</span><span class="sxs-lookup"><span data-stu-id="913f2-172">Whether the printer associated with this printer share is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="913f2-173">defaults</span><span class="sxs-lookup"><span data-stu-id="913f2-173">defaults</span></span>|[<span data-ttu-id="913f2-174">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="913f2-174">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="913f2-175">与此打印机共享关联的打印机的默认打印设置。</span><span class="sxs-lookup"><span data-stu-id="913f2-175">The default print settings of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="913f2-176">capabilities</span><span class="sxs-lookup"><span data-stu-id="913f2-176">capabilities</span></span>|[<span data-ttu-id="913f2-177">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="913f2-177">printerCapabilities</span></span>](printercapabilities.md)|<span data-ttu-id="913f2-178">与此打印机共享相关联的打印机的功能。</span><span class="sxs-lookup"><span data-stu-id="913f2-178">The capabilities of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="913f2-179">location</span><span class="sxs-lookup"><span data-stu-id="913f2-179">location</span></span>|[<span data-ttu-id="913f2-180">printerLocation</span><span class="sxs-lookup"><span data-stu-id="913f2-180">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="913f2-181">与此打印机共享关联的打印机的物理和/或组织位置。</span><span class="sxs-lookup"><span data-stu-id="913f2-181">The physical and/or organizational location of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="913f2-182">status</span><span class="sxs-lookup"><span data-stu-id="913f2-182">status</span></span>|[<span data-ttu-id="913f2-183">printerStatus</span><span class="sxs-lookup"><span data-stu-id="913f2-183">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="913f2-184">与此打印机共享关联的打印机的处理状态，包括任何错误。</span><span class="sxs-lookup"><span data-stu-id="913f2-184">The processing status, including any errors, of the printer associated with this printer share.</span></span> <span data-ttu-id="913f2-185">只读。</span><span class="sxs-lookup"><span data-stu-id="913f2-185">Read-only.</span></span>|
|<span data-ttu-id="913f2-186">allowAllUsers</span><span class="sxs-lookup"><span data-stu-id="913f2-186">allowAllUsers</span></span>|<span data-ttu-id="913f2-187">布尔</span><span class="sxs-lookup"><span data-stu-id="913f2-187">Boolean</span></span>|<span data-ttu-id="913f2-188">如果为 true，则所有用户和组都将被授予对此打印机共享的访问权限。</span><span class="sxs-lookup"><span data-stu-id="913f2-188">If true, all users and groups will be granted access to this printer share.</span></span> <span data-ttu-id="913f2-189">这将取代由 **allowedUsers** 和 **allowedGroups** 导航属性定义的允许列表。</span><span class="sxs-lookup"><span data-stu-id="913f2-189">This supersedes the allow lists defined by the **allowedUsers** and **allowedGroups** navigation properties.</span></span>|

## <a name="relationships"></a><span data-ttu-id="913f2-190">关系</span><span class="sxs-lookup"><span data-stu-id="913f2-190">Relationships</span></span>
| <span data-ttu-id="913f2-191">关系</span><span class="sxs-lookup"><span data-stu-id="913f2-191">Relationship</span></span> | <span data-ttu-id="913f2-192">类型</span><span class="sxs-lookup"><span data-stu-id="913f2-192">Type</span></span>        | <span data-ttu-id="913f2-193">说明</span><span class="sxs-lookup"><span data-stu-id="913f2-193">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="913f2-194">印刷</span><span class="sxs-lookup"><span data-stu-id="913f2-194">printer</span></span>|[<span data-ttu-id="913f2-195">印刷</span><span class="sxs-lookup"><span data-stu-id="913f2-195">printer</span></span>](printer.md)|<span data-ttu-id="913f2-196">与此打印机共享相关联的打印机。</span><span class="sxs-lookup"><span data-stu-id="913f2-196">The printer that this printer share is related to.</span></span> |
|<span data-ttu-id="913f2-197">allowedUsers</span><span class="sxs-lookup"><span data-stu-id="913f2-197">allowedUsers</span></span>|<span data-ttu-id="913f2-198">[printUserIdentity](printuseridentity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="913f2-198">[printUserIdentity](printuseridentity.md) collection</span></span>|<span data-ttu-id="913f2-199">有权使用打印机打印的用户。</span><span class="sxs-lookup"><span data-stu-id="913f2-199">The users who have access to print using the printer.</span></span>|
|<span data-ttu-id="913f2-200">allowedGroups</span><span class="sxs-lookup"><span data-stu-id="913f2-200">allowedGroups</span></span>|[<span data-ttu-id="913f2-201">printIdentity</span><span class="sxs-lookup"><span data-stu-id="913f2-201">printIdentity</span></span>](printidentity.md)|<span data-ttu-id="913f2-202">其用户有权使用打印机打印的组。</span><span class="sxs-lookup"><span data-stu-id="913f2-202">The groups whose users have access to print using the printer.</span></span>|
|<span data-ttu-id="913f2-203">jobs</span><span class="sxs-lookup"><span data-stu-id="913f2-203">jobs</span></span>|<span data-ttu-id="913f2-204">[printJob](printjob.md) 集合</span><span class="sxs-lookup"><span data-stu-id="913f2-204">[printJob](printjob.md) collection</span></span>| <span data-ttu-id="913f2-205">与此打印机共享关联的打印机排队等待打印的作业列表。</span><span class="sxs-lookup"><span data-stu-id="913f2-205">The list of jobs that are queued for printing by the printer associated with this printer share.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="913f2-206">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="913f2-206">JSON representation</span></span>

<span data-ttu-id="913f2-207">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="913f2-207">The following is a JSON representation of the resource.</span></span>

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
  "name": "String",
  "createdDateTime": "String (timestamp)"
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


