---
title: printerShare 资源类型
description: 表示可供用户和打印应用程序发现的打印机。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 5acbcdc58b730404a39af1f3069b3433fac54ed3
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44217345"
---
# <a name="printershare-resource-type"></a><span data-ttu-id="95774-103">printerShare 资源类型</span><span class="sxs-lookup"><span data-stu-id="95774-103">printerShare resource type</span></span>

<span data-ttu-id="95774-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95774-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95774-105">表示可供用户和打印应用程序发现的打印机。</span><span class="sxs-lookup"><span data-stu-id="95774-105">Represents a printer that is intended to be discoverable by users and printing applications.</span></span>

## <a name="methods"></a><span data-ttu-id="95774-106">Methods</span><span class="sxs-lookup"><span data-stu-id="95774-106">Methods</span></span>

| <span data-ttu-id="95774-107">方法</span><span class="sxs-lookup"><span data-stu-id="95774-107">Method</span></span>       | <span data-ttu-id="95774-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="95774-108">Return Type</span></span> | <span data-ttu-id="95774-109">说明</span><span class="sxs-lookup"><span data-stu-id="95774-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="95774-110">List</span><span class="sxs-lookup"><span data-stu-id="95774-110">List</span></span>](../api/print-list-shares.md) | <span data-ttu-id="95774-111">[printerShare](printershare.md)集合</span><span class="sxs-lookup"><span data-stu-id="95774-111">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="95774-112">获取租户中的打印机共享的列表。</span><span class="sxs-lookup"><span data-stu-id="95774-112">Get a list of printer shares in the tenant.</span></span> |
| [<span data-ttu-id="95774-113">获取</span><span class="sxs-lookup"><span data-stu-id="95774-113">Get</span></span>](../api/printershare-get.md) | [<span data-ttu-id="95774-114">printerShare</span><span class="sxs-lookup"><span data-stu-id="95774-114">printerShare</span></span>](printershare.md) | <span data-ttu-id="95774-115">读取**printerShare**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="95774-115">Read properties and relationships of a **printerShare** object.</span></span> |
| [<span data-ttu-id="95774-116">更新</span><span class="sxs-lookup"><span data-stu-id="95774-116">Update</span></span>](../api/printershare-update.md) | [<span data-ttu-id="95774-117">printerShare</span><span class="sxs-lookup"><span data-stu-id="95774-117">printerShare</span></span>](printershare.md) | <span data-ttu-id="95774-118">更新**printerShare**对象。</span><span class="sxs-lookup"><span data-stu-id="95774-118">Update a **printerShare** object.</span></span> |
| [<span data-ttu-id="95774-119">删除</span><span class="sxs-lookup"><span data-stu-id="95774-119">Delete</span></span>](../api/printershare-delete.md) | <span data-ttu-id="95774-120">无</span><span class="sxs-lookup"><span data-stu-id="95774-120">None</span></span> | <span data-ttu-id="95774-121">取消打印机的共享。</span><span class="sxs-lookup"><span data-stu-id="95774-121">Unshare a printer.</span></span> |
| [<span data-ttu-id="95774-122">列出 allowedUsers</span><span class="sxs-lookup"><span data-stu-id="95774-122">List allowedUsers</span></span>](../api/printershare-list-allowedusers.md) | <span data-ttu-id="95774-123">[printUserIdentity](printuseridentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="95774-123">[printUserIdentity](printuseridentity.md) collection</span></span> | <span data-ttu-id="95774-124">检索已授予访问权限以将打印作业提交到关联的打印机共享的用户列表。</span><span class="sxs-lookup"><span data-stu-id="95774-124">Retrieve a list of users who have been granted access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="95774-125">添加 allowedUser</span><span class="sxs-lookup"><span data-stu-id="95774-125">Add allowedUser</span></span>](../api/printershare-post-allowedusers.md) | <span data-ttu-id="95774-126">无</span><span class="sxs-lookup"><span data-stu-id="95774-126">None</span></span> | <span data-ttu-id="95774-127">向指定的用户授予将打印作业提交到关联的打印机共享的权限。</span><span class="sxs-lookup"><span data-stu-id="95774-127">Grant the specified user access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="95774-128">删除 allowedUser</span><span class="sxs-lookup"><span data-stu-id="95774-128">Remove allowedUser</span></span>](../api/printershare-delete-alloweduser.md) | <span data-ttu-id="95774-129">无</span><span class="sxs-lookup"><span data-stu-id="95774-129">None</span></span> | <span data-ttu-id="95774-130">撤销指定用户的打印机共享访问权限。</span><span class="sxs-lookup"><span data-stu-id="95774-130">Revoke printer share access from the specified user.</span></span> |
| [<span data-ttu-id="95774-131">列出 allowedGroups</span><span class="sxs-lookup"><span data-stu-id="95774-131">List allowedGroups</span></span>](../api/printershare-list-allowedgroups.md) | <span data-ttu-id="95774-132">[printIdentity](printidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="95774-132">[printIdentity](printidentity.md) collection</span></span> | <span data-ttu-id="95774-133">检索已授予访问权限的组列表，以将打印作业提交到关联的打印机共享。</span><span class="sxs-lookup"><span data-stu-id="95774-133">Retrieve a list of groups that have been granted access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="95774-134">添加 allowedGroup</span><span class="sxs-lookup"><span data-stu-id="95774-134">Add allowedGroup</span></span>](../api/printershare-post-allowedgroups.md) | <span data-ttu-id="95774-135">无</span><span class="sxs-lookup"><span data-stu-id="95774-135">None</span></span> | <span data-ttu-id="95774-136">向指定的组授予将打印作业提交到关联的打印机共享的权限。</span><span class="sxs-lookup"><span data-stu-id="95774-136">Grant the specified group access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="95774-137">删除 allowedGroup</span><span class="sxs-lookup"><span data-stu-id="95774-137">Remove allowedGroup</span></span>](../api/printershare-delete-allowedgroup.md) | <span data-ttu-id="95774-138">无</span><span class="sxs-lookup"><span data-stu-id="95774-138">None</span></span> | <span data-ttu-id="95774-139">撤销指定组的打印机共享访问权限。</span><span class="sxs-lookup"><span data-stu-id="95774-139">Revoke printer share access from the specified group.</span></span> |

## <a name="properties"></a><span data-ttu-id="95774-140">属性</span><span class="sxs-lookup"><span data-stu-id="95774-140">Properties</span></span>
| <span data-ttu-id="95774-141">属性</span><span class="sxs-lookup"><span data-stu-id="95774-141">Property</span></span>     | <span data-ttu-id="95774-142">类型</span><span class="sxs-lookup"><span data-stu-id="95774-142">Type</span></span>        | <span data-ttu-id="95774-143">说明</span><span class="sxs-lookup"><span data-stu-id="95774-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="95774-144">id</span><span class="sxs-lookup"><span data-stu-id="95774-144">id</span></span>|<span data-ttu-id="95774-145">String</span><span class="sxs-lookup"><span data-stu-id="95774-145">String</span></span>| <span data-ttu-id="95774-146">PrinterShare 的标识符。</span><span class="sxs-lookup"><span data-stu-id="95774-146">The printerShare's identifier.</span></span> <span data-ttu-id="95774-147">只读。</span><span class="sxs-lookup"><span data-stu-id="95774-147">Read-only.</span></span>|
|<span data-ttu-id="95774-148">displayName</span><span class="sxs-lookup"><span data-stu-id="95774-148">displayName</span></span>|<span data-ttu-id="95774-149">字符串</span><span class="sxs-lookup"><span data-stu-id="95774-149">String</span></span>|<span data-ttu-id="95774-150">打印客户端应显示的打印机共享的名称。</span><span class="sxs-lookup"><span data-stu-id="95774-150">The name of the printer share that print clients should display.</span></span>|
|<span data-ttu-id="95774-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95774-151">createdDateTime</span></span>|<span data-ttu-id="95774-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95774-152">DateTimeOffset</span></span>|<span data-ttu-id="95774-153">创建打印机共享时的 DateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="95774-153">The DateTimeOffset when the printer share was created.</span></span> <span data-ttu-id="95774-154">只读。</span><span class="sxs-lookup"><span data-stu-id="95774-154">Read-only.</span></span>|
|<span data-ttu-id="95774-155">manufacturer</span><span class="sxs-lookup"><span data-stu-id="95774-155">manufacturer</span></span>|<span data-ttu-id="95774-156">String</span><span class="sxs-lookup"><span data-stu-id="95774-156">String</span></span>|<span data-ttu-id="95774-157">与此打印机共享关联的打印机报告的制造商。</span><span class="sxs-lookup"><span data-stu-id="95774-157">The manufacturer reported by the printer associated with this printer share.</span></span> <span data-ttu-id="95774-158">只读。</span><span class="sxs-lookup"><span data-stu-id="95774-158">Read-only.</span></span>|
|<span data-ttu-id="95774-159">model</span><span class="sxs-lookup"><span data-stu-id="95774-159">model</span></span>|<span data-ttu-id="95774-160">String</span><span class="sxs-lookup"><span data-stu-id="95774-160">String</span></span>|<span data-ttu-id="95774-161">与此打印机共享关联的打印机报告的模型名称。</span><span class="sxs-lookup"><span data-stu-id="95774-161">The model name reported by the printer associated with this printer share.</span></span> <span data-ttu-id="95774-162">只读。</span><span class="sxs-lookup"><span data-stu-id="95774-162">Read-only.</span></span>|
|<span data-ttu-id="95774-163">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="95774-163">isAcceptingJobs</span></span>|<span data-ttu-id="95774-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="95774-164">Boolean</span></span>|<span data-ttu-id="95774-165">与此打印机共享关联的打印机当前是否正在接受新的打印作业。</span><span class="sxs-lookup"><span data-stu-id="95774-165">Whether the printer associated with this printer share is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="95774-166">缺省值</span><span class="sxs-lookup"><span data-stu-id="95774-166">defaults</span></span>|[<span data-ttu-id="95774-167">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="95774-167">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="95774-168">与此打印机共享关联的打印机的默认打印设置。</span><span class="sxs-lookup"><span data-stu-id="95774-168">The default print settings of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="95774-169">capabilities</span><span class="sxs-lookup"><span data-stu-id="95774-169">capabilities</span></span>|[<span data-ttu-id="95774-170">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="95774-170">printerCapabilities</span></span>](printercapabilities.md)|<span data-ttu-id="95774-171">与此打印机共享相关联的打印机的功能。</span><span class="sxs-lookup"><span data-stu-id="95774-171">The capabilities of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="95774-172">位置</span><span class="sxs-lookup"><span data-stu-id="95774-172">location</span></span>|[<span data-ttu-id="95774-173">printerLocation</span><span class="sxs-lookup"><span data-stu-id="95774-173">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="95774-174">与此打印机共享关联的打印机的物理和/或组织位置。</span><span class="sxs-lookup"><span data-stu-id="95774-174">The physical and/or organizational location of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="95774-175">status</span><span class="sxs-lookup"><span data-stu-id="95774-175">status</span></span>|[<span data-ttu-id="95774-176">printerStatus</span><span class="sxs-lookup"><span data-stu-id="95774-176">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="95774-177">与此打印机共享关联的打印机的处理状态，包括任何错误。</span><span class="sxs-lookup"><span data-stu-id="95774-177">The processing status, including any errors, of the printer associated with this printer share.</span></span> <span data-ttu-id="95774-178">只读。</span><span class="sxs-lookup"><span data-stu-id="95774-178">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95774-179">关系</span><span class="sxs-lookup"><span data-stu-id="95774-179">Relationships</span></span>
| <span data-ttu-id="95774-180">关系</span><span class="sxs-lookup"><span data-stu-id="95774-180">Relationship</span></span> | <span data-ttu-id="95774-181">类型</span><span class="sxs-lookup"><span data-stu-id="95774-181">Type</span></span>        | <span data-ttu-id="95774-182">说明</span><span class="sxs-lookup"><span data-stu-id="95774-182">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="95774-183">印刷</span><span class="sxs-lookup"><span data-stu-id="95774-183">printer</span></span>|[<span data-ttu-id="95774-184">印刷</span><span class="sxs-lookup"><span data-stu-id="95774-184">printer</span></span>](printer.md)|<span data-ttu-id="95774-185">与此打印机共享相关联的打印机。</span><span class="sxs-lookup"><span data-stu-id="95774-185">The printer that this printer share is related to.</span></span> |
|<span data-ttu-id="95774-186">allowedUsers</span><span class="sxs-lookup"><span data-stu-id="95774-186">allowedUsers</span></span>|<span data-ttu-id="95774-187">[printUserIdentity](printuseridentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="95774-187">[printUserIdentity](printuseridentity.md) collection</span></span>|<span data-ttu-id="95774-188">有权使用打印机打印的用户。</span><span class="sxs-lookup"><span data-stu-id="95774-188">The users who have access to print using the printer.</span></span>|
|<span data-ttu-id="95774-189">allowedGroups</span><span class="sxs-lookup"><span data-stu-id="95774-189">allowedGroups</span></span>|[<span data-ttu-id="95774-190">printIdentity</span><span class="sxs-lookup"><span data-stu-id="95774-190">printIdentity</span></span>](printidentity.md)|<span data-ttu-id="95774-191">其用户有权使用打印机打印的组。</span><span class="sxs-lookup"><span data-stu-id="95774-191">The groups whose users have access to print using the printer.</span></span>|
|<span data-ttu-id="95774-192">jobs</span><span class="sxs-lookup"><span data-stu-id="95774-192">jobs</span></span>|<span data-ttu-id="95774-193">[printJob](printjob.md)集合</span><span class="sxs-lookup"><span data-stu-id="95774-193">[printJob](printjob.md) collection</span></span>| <span data-ttu-id="95774-194">与此打印机共享关联的打印机排队等待打印的作业列表。</span><span class="sxs-lookup"><span data-stu-id="95774-194">The list of jobs that are queued for printing by the printer associated with this printer share.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="95774-195">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="95774-195">JSON representation</span></span>

<span data-ttu-id="95774-196">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95774-196">The following is a JSON representation of the resource.</span></span>

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
