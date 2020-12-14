---
title: printerShare 资源类型
description: 表示供用户和打印应用程序发现的打印机。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 5f8b8ad8446d37c73ddfd2b55b8ca544f1f926cd
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49664073"
---
# <a name="printershare-resource-type"></a><span data-ttu-id="43fc9-103">printerShare 资源类型</span><span class="sxs-lookup"><span data-stu-id="43fc9-103">printerShare resource type</span></span>

<span data-ttu-id="43fc9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43fc9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43fc9-105">表示供用户和打印应用程序发现的打印机。</span><span class="sxs-lookup"><span data-stu-id="43fc9-105">Represents a printer that is intended to be discoverable by users and printing applications.</span></span>

## <a name="methods"></a><span data-ttu-id="43fc9-106">方法</span><span class="sxs-lookup"><span data-stu-id="43fc9-106">Methods</span></span>

| <span data-ttu-id="43fc9-107">方法</span><span class="sxs-lookup"><span data-stu-id="43fc9-107">Method</span></span>       | <span data-ttu-id="43fc9-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="43fc9-108">Return Type</span></span> | <span data-ttu-id="43fc9-109">Description</span><span class="sxs-lookup"><span data-stu-id="43fc9-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="43fc9-110">List</span><span class="sxs-lookup"><span data-stu-id="43fc9-110">List</span></span>](../api/print-list-shares.md) | <span data-ttu-id="43fc9-111">[printerShare](printershare.md) 集合</span><span class="sxs-lookup"><span data-stu-id="43fc9-111">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="43fc9-112">获取租户中打印机共享的列表。</span><span class="sxs-lookup"><span data-stu-id="43fc9-112">Get a list of printer shares in the tenant.</span></span> |
| [<span data-ttu-id="43fc9-113">获取</span><span class="sxs-lookup"><span data-stu-id="43fc9-113">Get</span></span>](../api/printershare-get.md) | [<span data-ttu-id="43fc9-114">printerShare</span><span class="sxs-lookup"><span data-stu-id="43fc9-114">printerShare</span></span>](printershare.md) | <span data-ttu-id="43fc9-115">读取 **printerShare** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="43fc9-115">Read properties and relationships of a **printerShare** object.</span></span> |
| [<span data-ttu-id="43fc9-116">更新</span><span class="sxs-lookup"><span data-stu-id="43fc9-116">Update</span></span>](../api/printershare-update.md) | [<span data-ttu-id="43fc9-117">printerShare</span><span class="sxs-lookup"><span data-stu-id="43fc9-117">printerShare</span></span>](printershare.md) | <span data-ttu-id="43fc9-118">更新 **printerShare** 对象。</span><span class="sxs-lookup"><span data-stu-id="43fc9-118">Update a **printerShare** object.</span></span> |
| [<span data-ttu-id="43fc9-119">删除</span><span class="sxs-lookup"><span data-stu-id="43fc9-119">Delete</span></span>](../api/printershare-delete.md) | <span data-ttu-id="43fc9-120">无</span><span class="sxs-lookup"><span data-stu-id="43fc9-120">None</span></span> | <span data-ttu-id="43fc9-121">取消共享打印机。</span><span class="sxs-lookup"><span data-stu-id="43fc9-121">Unshare a printer.</span></span> |
| [<span data-ttu-id="43fc9-122">列出作业</span><span class="sxs-lookup"><span data-stu-id="43fc9-122">List jobs</span></span>](../api/printershare-list-jobs.md) | <span data-ttu-id="43fc9-123">[printJob](printjob.md) 集合</span><span class="sxs-lookup"><span data-stu-id="43fc9-123">[printJob](printjob.md) collection</span></span> | <span data-ttu-id="43fc9-124">获取由 printerShare 排队进行处理的打印作业列表。</span><span class="sxs-lookup"><span data-stu-id="43fc9-124">Get a list of print jobs that are queued for processing by the printerShare.</span></span> |
| [<span data-ttu-id="43fc9-125">创建作业</span><span class="sxs-lookup"><span data-stu-id="43fc9-125">Create job</span></span>](../api/printershare-post-jobs.md) | [<span data-ttu-id="43fc9-126">printJob</span><span class="sxs-lookup"><span data-stu-id="43fc9-126">printJob</span></span>](printjob.md) | <span data-ttu-id="43fc9-127">为 printerShare 创建新的打印作业。</span><span class="sxs-lookup"><span data-stu-id="43fc9-127">Create a new print job for the printerShare.</span></span> <span data-ttu-id="43fc9-128">若要开始打印作业，请使用"开始["。](../api/printjob-start.md)</span><span class="sxs-lookup"><span data-stu-id="43fc9-128">To start printing the job, use [start](../api/printjob-start.md).</span></span> |
| [<span data-ttu-id="43fc9-129">列出 allowedUsers</span><span class="sxs-lookup"><span data-stu-id="43fc9-129">List allowedUsers</span></span>](../api/printershare-list-allowedusers.md) | <span data-ttu-id="43fc9-130">[user](user.md) 集合</span><span class="sxs-lookup"><span data-stu-id="43fc9-130">[user](user.md) collection</span></span> | <span data-ttu-id="43fc9-131">检索已被授予将打印作业提交到关联的打印机共享的访问权限的用户列表。</span><span class="sxs-lookup"><span data-stu-id="43fc9-131">Retrieve a list of users who have been granted access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="43fc9-132">添加 allowedUser</span><span class="sxs-lookup"><span data-stu-id="43fc9-132">Add allowedUser</span></span>](../api/printershare-post-allowedusers.md) | <span data-ttu-id="43fc9-133">无</span><span class="sxs-lookup"><span data-stu-id="43fc9-133">None</span></span> | <span data-ttu-id="43fc9-134">向指定的用户授予将打印作业提交到关联的打印机共享的权限。</span><span class="sxs-lookup"><span data-stu-id="43fc9-134">Grant the specified user access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="43fc9-135">删除 allowedUser</span><span class="sxs-lookup"><span data-stu-id="43fc9-135">Remove allowedUser</span></span>](../api/printershare-delete-alloweduser.md) | <span data-ttu-id="43fc9-136">无</span><span class="sxs-lookup"><span data-stu-id="43fc9-136">None</span></span> | <span data-ttu-id="43fc9-137">撤销指定用户的打印机共享访问权限。</span><span class="sxs-lookup"><span data-stu-id="43fc9-137">Revoke printer share access from the specified user.</span></span> |
| [<span data-ttu-id="43fc9-138">列出 allowedGroups</span><span class="sxs-lookup"><span data-stu-id="43fc9-138">List allowedGroups</span></span>](../api/printershare-list-allowedgroups.md) | <span data-ttu-id="43fc9-139">[group](group.md) 集合</span><span class="sxs-lookup"><span data-stu-id="43fc9-139">[group](group.md) collection</span></span> | <span data-ttu-id="43fc9-140">检索已被授予将打印作业提交到关联的打印机共享的访问权限的组列表。</span><span class="sxs-lookup"><span data-stu-id="43fc9-140">Retrieve a list of groups that have been granted access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="43fc9-141">添加 allowedGroup</span><span class="sxs-lookup"><span data-stu-id="43fc9-141">Add allowedGroup</span></span>](../api/printershare-post-allowedgroups.md) | <span data-ttu-id="43fc9-142">无</span><span class="sxs-lookup"><span data-stu-id="43fc9-142">None</span></span> | <span data-ttu-id="43fc9-143">授予指定的组访问权限，以将打印作业提交到关联的打印机共享。</span><span class="sxs-lookup"><span data-stu-id="43fc9-143">Grant the specified group access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="43fc9-144">删除 allowedGroup</span><span class="sxs-lookup"><span data-stu-id="43fc9-144">Remove allowedGroup</span></span>](../api/printershare-delete-allowedgroup.md) | <span data-ttu-id="43fc9-145">无</span><span class="sxs-lookup"><span data-stu-id="43fc9-145">None</span></span> | <span data-ttu-id="43fc9-146">撤销指定组的打印机共享访问权限。</span><span class="sxs-lookup"><span data-stu-id="43fc9-146">Revoke printer share access from the specified group.</span></span> |

## <a name="properties"></a><span data-ttu-id="43fc9-147">属性</span><span class="sxs-lookup"><span data-stu-id="43fc9-147">Properties</span></span>
| <span data-ttu-id="43fc9-148">属性</span><span class="sxs-lookup"><span data-stu-id="43fc9-148">Property</span></span>     | <span data-ttu-id="43fc9-149">类型</span><span class="sxs-lookup"><span data-stu-id="43fc9-149">Type</span></span>        | <span data-ttu-id="43fc9-150">说明</span><span class="sxs-lookup"><span data-stu-id="43fc9-150">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="43fc9-151">id</span><span class="sxs-lookup"><span data-stu-id="43fc9-151">id</span></span>|<span data-ttu-id="43fc9-152">String</span><span class="sxs-lookup"><span data-stu-id="43fc9-152">String</span></span>| <span data-ttu-id="43fc9-153">printerShare 的标识符。</span><span class="sxs-lookup"><span data-stu-id="43fc9-153">The printerShare's identifier.</span></span> <span data-ttu-id="43fc9-154">只读。</span><span class="sxs-lookup"><span data-stu-id="43fc9-154">Read-only.</span></span>|
|<span data-ttu-id="43fc9-155">displayName</span><span class="sxs-lookup"><span data-stu-id="43fc9-155">displayName</span></span>|<span data-ttu-id="43fc9-156">String</span><span class="sxs-lookup"><span data-stu-id="43fc9-156">String</span></span>|<span data-ttu-id="43fc9-157">打印客户端应显示的打印机共享的名称。</span><span class="sxs-lookup"><span data-stu-id="43fc9-157">The name of the printer share that print clients should display.</span></span>|
|<span data-ttu-id="43fc9-158">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="43fc9-158">createdDateTime</span></span>|<span data-ttu-id="43fc9-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43fc9-159">DateTimeOffset</span></span>|<span data-ttu-id="43fc9-160">创建打印机共享时的日期时间Offset。</span><span class="sxs-lookup"><span data-stu-id="43fc9-160">The DateTimeOffset when the printer share was created.</span></span> <span data-ttu-id="43fc9-161">只读。</span><span class="sxs-lookup"><span data-stu-id="43fc9-161">Read-only.</span></span>|
|<span data-ttu-id="43fc9-162">manufacturer</span><span class="sxs-lookup"><span data-stu-id="43fc9-162">manufacturer</span></span>|<span data-ttu-id="43fc9-163">String</span><span class="sxs-lookup"><span data-stu-id="43fc9-163">String</span></span>|<span data-ttu-id="43fc9-164">与此打印机共享关联的打印机报告的制造商。</span><span class="sxs-lookup"><span data-stu-id="43fc9-164">The manufacturer reported by the printer associated with this printer share.</span></span> <span data-ttu-id="43fc9-165">只读。</span><span class="sxs-lookup"><span data-stu-id="43fc9-165">Read-only.</span></span>|
|<span data-ttu-id="43fc9-166">model</span><span class="sxs-lookup"><span data-stu-id="43fc9-166">model</span></span>|<span data-ttu-id="43fc9-167">String</span><span class="sxs-lookup"><span data-stu-id="43fc9-167">String</span></span>|<span data-ttu-id="43fc9-168">与此打印机共享关联的打印机报告的型号名称。</span><span class="sxs-lookup"><span data-stu-id="43fc9-168">The model name reported by the printer associated with this printer share.</span></span> <span data-ttu-id="43fc9-169">只读。</span><span class="sxs-lookup"><span data-stu-id="43fc9-169">Read-only.</span></span>|
|<span data-ttu-id="43fc9-170">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="43fc9-170">isAcceptingJobs</span></span>|<span data-ttu-id="43fc9-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="43fc9-171">Boolean</span></span>|<span data-ttu-id="43fc9-172">与此打印机共享关联的打印机当前是否接受新的打印作业。</span><span class="sxs-lookup"><span data-stu-id="43fc9-172">Whether the printer associated with this printer share is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="43fc9-173">defaults</span><span class="sxs-lookup"><span data-stu-id="43fc9-173">defaults</span></span>|[<span data-ttu-id="43fc9-174">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="43fc9-174">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="43fc9-175">与此打印机共享关联的打印机的默认打印设置。</span><span class="sxs-lookup"><span data-stu-id="43fc9-175">The default print settings of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="43fc9-176">capabilities</span><span class="sxs-lookup"><span data-stu-id="43fc9-176">capabilities</span></span>|[<span data-ttu-id="43fc9-177">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="43fc9-177">printerCapabilities</span></span>](printercapabilities.md)|<span data-ttu-id="43fc9-178">与此打印机共享关联的打印机的功能。</span><span class="sxs-lookup"><span data-stu-id="43fc9-178">The capabilities of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="43fc9-179">位置</span><span class="sxs-lookup"><span data-stu-id="43fc9-179">location</span></span>|[<span data-ttu-id="43fc9-180">printerLocation</span><span class="sxs-lookup"><span data-stu-id="43fc9-180">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="43fc9-181">与此打印机共享关联的打印机的物理和/或组织位置。</span><span class="sxs-lookup"><span data-stu-id="43fc9-181">The physical and/or organizational location of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="43fc9-182">status</span><span class="sxs-lookup"><span data-stu-id="43fc9-182">status</span></span>|[<span data-ttu-id="43fc9-183">printerStatus</span><span class="sxs-lookup"><span data-stu-id="43fc9-183">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="43fc9-184">与此打印机共享关联的打印机的处理状态（包括任何错误）。</span><span class="sxs-lookup"><span data-stu-id="43fc9-184">The processing status, including any errors, of the printer associated with this printer share.</span></span> <span data-ttu-id="43fc9-185">只读。</span><span class="sxs-lookup"><span data-stu-id="43fc9-185">Read-only.</span></span>|
|<span data-ttu-id="43fc9-186">allowAllUsers</span><span class="sxs-lookup"><span data-stu-id="43fc9-186">allowAllUsers</span></span>|<span data-ttu-id="43fc9-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="43fc9-187">Boolean</span></span>|<span data-ttu-id="43fc9-188">如果为 true，将授予所有用户和组对此打印机共享的访问权限。</span><span class="sxs-lookup"><span data-stu-id="43fc9-188">If true, all users and groups will be granted access to this printer share.</span></span> <span data-ttu-id="43fc9-189">这将取代 **allowedUsers** 和 **allowedGroups** 导航属性定义的允许列表。</span><span class="sxs-lookup"><span data-stu-id="43fc9-189">This supersedes the allow lists defined by the **allowedUsers** and **allowedGroups** navigation properties.</span></span>|

## <a name="relationships"></a><span data-ttu-id="43fc9-190">关系</span><span class="sxs-lookup"><span data-stu-id="43fc9-190">Relationships</span></span>
| <span data-ttu-id="43fc9-191">关系</span><span class="sxs-lookup"><span data-stu-id="43fc9-191">Relationship</span></span> | <span data-ttu-id="43fc9-192">类型</span><span class="sxs-lookup"><span data-stu-id="43fc9-192">Type</span></span>        | <span data-ttu-id="43fc9-193">说明</span><span class="sxs-lookup"><span data-stu-id="43fc9-193">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="43fc9-194">printer</span><span class="sxs-lookup"><span data-stu-id="43fc9-194">printer</span></span>|[<span data-ttu-id="43fc9-195">printer</span><span class="sxs-lookup"><span data-stu-id="43fc9-195">printer</span></span>](printer.md)|<span data-ttu-id="43fc9-196">此打印机共享相关的打印机。</span><span class="sxs-lookup"><span data-stu-id="43fc9-196">The printer that this printer share is related to.</span></span> |
|<span data-ttu-id="43fc9-197">allowedUsers</span><span class="sxs-lookup"><span data-stu-id="43fc9-197">allowedUsers</span></span>|<span data-ttu-id="43fc9-198">[user](user.md) 集合</span><span class="sxs-lookup"><span data-stu-id="43fc9-198">[user](user.md) collection</span></span>|<span data-ttu-id="43fc9-199">有权访问使用打印机打印的用户。</span><span class="sxs-lookup"><span data-stu-id="43fc9-199">The users who have access to print using the printer.</span></span>|
|<span data-ttu-id="43fc9-200">allowedGroups</span><span class="sxs-lookup"><span data-stu-id="43fc9-200">allowedGroups</span></span>|[<span data-ttu-id="43fc9-201">组</span><span class="sxs-lookup"><span data-stu-id="43fc9-201">group</span></span>](group.md)|<span data-ttu-id="43fc9-202">用户有权访问使用打印机打印的组。</span><span class="sxs-lookup"><span data-stu-id="43fc9-202">The groups whose users have access to print using the printer.</span></span>|
|<span data-ttu-id="43fc9-203">jobs</span><span class="sxs-lookup"><span data-stu-id="43fc9-203">jobs</span></span>|<span data-ttu-id="43fc9-204">[printJob](printjob.md) 集合</span><span class="sxs-lookup"><span data-stu-id="43fc9-204">[printJob](printjob.md) collection</span></span>| <span data-ttu-id="43fc9-205">由与此打印机共享关联的打印机排入打印队列的作业列表。</span><span class="sxs-lookup"><span data-stu-id="43fc9-205">The list of jobs that are queued for printing by the printer associated with this printer share.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="43fc9-206">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="43fc9-206">JSON representation</span></span>

<span data-ttu-id="43fc9-207">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="43fc9-207">The following is a JSON representation of the resource.</span></span>

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


