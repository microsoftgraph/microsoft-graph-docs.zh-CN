---
title: printerShare 资源类型
description: 表示可供用户和打印应用程序发现的打印机。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 8aa9312bf8b7e8f9a2cec049b8275d4ce7a04012
ms.sourcegitcommit: 195fa0d441a49662e144323d37518dbba0c76fc7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2020
ms.locfileid: "43806843"
---
# <a name="printershare-resource-type"></a><span data-ttu-id="7eba6-103">printerShare 资源类型</span><span class="sxs-lookup"><span data-stu-id="7eba6-103">printerShare resource type</span></span>

<span data-ttu-id="7eba6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7eba6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7eba6-105">表示可供用户和打印应用程序发现的打印机。</span><span class="sxs-lookup"><span data-stu-id="7eba6-105">Represents a printer that is intended to be discoverable by users and printing applications.</span></span>

## <a name="methods"></a><span data-ttu-id="7eba6-106">Methods</span><span class="sxs-lookup"><span data-stu-id="7eba6-106">Methods</span></span>

| <span data-ttu-id="7eba6-107">方法</span><span class="sxs-lookup"><span data-stu-id="7eba6-107">Method</span></span>       | <span data-ttu-id="7eba6-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="7eba6-108">Return Type</span></span> | <span data-ttu-id="7eba6-109">说明</span><span class="sxs-lookup"><span data-stu-id="7eba6-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="7eba6-110">List</span><span class="sxs-lookup"><span data-stu-id="7eba6-110">List</span></span>](../api/print-list-printershares.md) | <span data-ttu-id="7eba6-111">[printerShare](printershare.md)集合</span><span class="sxs-lookup"><span data-stu-id="7eba6-111">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="7eba6-112">获取租户中的打印机共享的列表。</span><span class="sxs-lookup"><span data-stu-id="7eba6-112">Get a list of printer shares in the tenant.</span></span> |
| [<span data-ttu-id="7eba6-113">获取</span><span class="sxs-lookup"><span data-stu-id="7eba6-113">Get</span></span>](../api/printershare-get.md) | [<span data-ttu-id="7eba6-114">printerShare</span><span class="sxs-lookup"><span data-stu-id="7eba6-114">printerShare</span></span>](printershare.md) | <span data-ttu-id="7eba6-115">读取**printerShare**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7eba6-115">Read properties and relationships of a **printerShare** object.</span></span> |
| [<span data-ttu-id="7eba6-116">更新</span><span class="sxs-lookup"><span data-stu-id="7eba6-116">Update</span></span>](../api/printershare-update.md) | [<span data-ttu-id="7eba6-117">printerShare</span><span class="sxs-lookup"><span data-stu-id="7eba6-117">printerShare</span></span>](printershare.md) | <span data-ttu-id="7eba6-118">更新**printerShare**对象。</span><span class="sxs-lookup"><span data-stu-id="7eba6-118">Update a **printerShare** object.</span></span> |
| [<span data-ttu-id="7eba6-119">删除</span><span class="sxs-lookup"><span data-stu-id="7eba6-119">Delete</span></span>](../api/printershare-delete.md) | <span data-ttu-id="7eba6-120">无</span><span class="sxs-lookup"><span data-stu-id="7eba6-120">None</span></span> | <span data-ttu-id="7eba6-121">取消打印机的共享。</span><span class="sxs-lookup"><span data-stu-id="7eba6-121">Unshare a printer.</span></span> |
| [<span data-ttu-id="7eba6-122">列出 allowedUsers</span><span class="sxs-lookup"><span data-stu-id="7eba6-122">List allowedUsers</span></span>](../api/printershare-list-allowedusers.md) | <span data-ttu-id="7eba6-123">[userIdentity](useridentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="7eba6-123">[userIdentity](useridentity.md) collection</span></span> | <span data-ttu-id="7eba6-124">检索已授予访问权限以将打印作业提交到关联的打印机共享的用户列表。</span><span class="sxs-lookup"><span data-stu-id="7eba6-124">Retrieve a list of users who have been granted access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="7eba6-125">添加 allowedUser</span><span class="sxs-lookup"><span data-stu-id="7eba6-125">Add allowedUser</span></span>](../api/printershare-post-allowedusers.md) | <span data-ttu-id="7eba6-126">无</span><span class="sxs-lookup"><span data-stu-id="7eba6-126">None</span></span> | <span data-ttu-id="7eba6-127">向指定的用户授予将打印作业提交到关联的打印机共享的权限。</span><span class="sxs-lookup"><span data-stu-id="7eba6-127">Grant the specified user access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="7eba6-128">删除 allowedUser</span><span class="sxs-lookup"><span data-stu-id="7eba6-128">Remove allowedUser</span></span>](../api/printershare-delete-alloweduser.md) | <span data-ttu-id="7eba6-129">无</span><span class="sxs-lookup"><span data-stu-id="7eba6-129">None</span></span> | <span data-ttu-id="7eba6-130">撤销指定用户的打印机共享访问权限。</span><span class="sxs-lookup"><span data-stu-id="7eba6-130">Revoke printer share access from the specified user.</span></span> |
| [<span data-ttu-id="7eba6-131">列出 allowedGroups</span><span class="sxs-lookup"><span data-stu-id="7eba6-131">List allowedGroups</span></span>](../api/printershare-list-allowedgroups.md) | <span data-ttu-id="7eba6-132">[标识](identity.md)集合</span><span class="sxs-lookup"><span data-stu-id="7eba6-132">[identity](identity.md) collection</span></span> | <span data-ttu-id="7eba6-133">检索已授予访问权限的组列表，以将打印作业提交到关联的打印机共享。</span><span class="sxs-lookup"><span data-stu-id="7eba6-133">Retrieve a list of groups that have been granted access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="7eba6-134">添加 allowedGroup</span><span class="sxs-lookup"><span data-stu-id="7eba6-134">Add allowedGroup</span></span>](../api/printershare-post-allowedgroups.md) | <span data-ttu-id="7eba6-135">无</span><span class="sxs-lookup"><span data-stu-id="7eba6-135">None</span></span> | <span data-ttu-id="7eba6-136">向指定的组授予将打印作业提交到关联的打印机共享的权限。</span><span class="sxs-lookup"><span data-stu-id="7eba6-136">Grant the specified group access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="7eba6-137">删除 allowedGroup</span><span class="sxs-lookup"><span data-stu-id="7eba6-137">Remove allowedGroup</span></span>](../api/printershare-delete-allowedgroup.md) | <span data-ttu-id="7eba6-138">无</span><span class="sxs-lookup"><span data-stu-id="7eba6-138">None</span></span> | <span data-ttu-id="7eba6-139">撤销指定组的打印机共享访问权限。</span><span class="sxs-lookup"><span data-stu-id="7eba6-139">Revoke printer share access from the specified group.</span></span> |

## <a name="properties"></a><span data-ttu-id="7eba6-140">属性</span><span class="sxs-lookup"><span data-stu-id="7eba6-140">Properties</span></span>
| <span data-ttu-id="7eba6-141">属性</span><span class="sxs-lookup"><span data-stu-id="7eba6-141">Property</span></span>     | <span data-ttu-id="7eba6-142">类型</span><span class="sxs-lookup"><span data-stu-id="7eba6-142">Type</span></span>        | <span data-ttu-id="7eba6-143">说明</span><span class="sxs-lookup"><span data-stu-id="7eba6-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7eba6-144">id</span><span class="sxs-lookup"><span data-stu-id="7eba6-144">id</span></span>|<span data-ttu-id="7eba6-145">String</span><span class="sxs-lookup"><span data-stu-id="7eba6-145">String</span></span>| <span data-ttu-id="7eba6-146">PrinterShare 的标识符。</span><span class="sxs-lookup"><span data-stu-id="7eba6-146">The printerShare's identifier.</span></span> <span data-ttu-id="7eba6-147">只读。</span><span class="sxs-lookup"><span data-stu-id="7eba6-147">Read-only.</span></span>|
|<span data-ttu-id="7eba6-148">name</span><span class="sxs-lookup"><span data-stu-id="7eba6-148">name</span></span>|<span data-ttu-id="7eba6-149">字符串</span><span class="sxs-lookup"><span data-stu-id="7eba6-149">String</span></span>|<span data-ttu-id="7eba6-150">打印客户端应显示的打印机共享的名称。</span><span class="sxs-lookup"><span data-stu-id="7eba6-150">The name of the printer share that print clients should display.</span></span>|
|<span data-ttu-id="7eba6-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7eba6-151">createdDateTime</span></span>|<span data-ttu-id="7eba6-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7eba6-152">DateTimeOffset</span></span>|<span data-ttu-id="7eba6-153">创建打印机共享时的 DateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="7eba6-153">The DateTimeOffset when the printer share was created.</span></span> <span data-ttu-id="7eba6-154">只读。</span><span class="sxs-lookup"><span data-stu-id="7eba6-154">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7eba6-155">关系</span><span class="sxs-lookup"><span data-stu-id="7eba6-155">Relationships</span></span>
| <span data-ttu-id="7eba6-156">关系</span><span class="sxs-lookup"><span data-stu-id="7eba6-156">Relationship</span></span> | <span data-ttu-id="7eba6-157">类型</span><span class="sxs-lookup"><span data-stu-id="7eba6-157">Type</span></span>        | <span data-ttu-id="7eba6-158">说明</span><span class="sxs-lookup"><span data-stu-id="7eba6-158">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7eba6-159">印刷</span><span class="sxs-lookup"><span data-stu-id="7eba6-159">printer</span></span>|[<span data-ttu-id="7eba6-160">印刷</span><span class="sxs-lookup"><span data-stu-id="7eba6-160">printer</span></span>](printer.md)|<span data-ttu-id="7eba6-161">与此打印机共享相关联的打印机。</span><span class="sxs-lookup"><span data-stu-id="7eba6-161">The printer that this printer share is related to.</span></span> |
|<span data-ttu-id="7eba6-162">allowedUsers</span><span class="sxs-lookup"><span data-stu-id="7eba6-162">allowedUsers</span></span>|<span data-ttu-id="7eba6-163">[userIdentity](useridentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="7eba6-163">[userIdentity](useridentity.md) collection</span></span>|<span data-ttu-id="7eba6-164">有权使用打印机打印的用户。</span><span class="sxs-lookup"><span data-stu-id="7eba6-164">The users who have access to print using the printer.</span></span>|
|<span data-ttu-id="7eba6-165">allowedGroups</span><span class="sxs-lookup"><span data-stu-id="7eba6-165">allowedGroups</span></span>|[<span data-ttu-id="7eba6-166">identity</span><span class="sxs-lookup"><span data-stu-id="7eba6-166">identity</span></span>](identity.md)|<span data-ttu-id="7eba6-167">其用户有权使用打印机打印的组。</span><span class="sxs-lookup"><span data-stu-id="7eba6-167">The groups whose users have access to print using the printer.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7eba6-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7eba6-168">JSON representation</span></span>

<span data-ttu-id="7eba6-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7eba6-169">The following is a JSON representation of the resource.</span></span>

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
