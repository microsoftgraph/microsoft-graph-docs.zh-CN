---
title: contactFolder 资源类型
description: 包含联系人的文件夹。
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 10e48459645c8af6d03787a3b2395398098cc7e0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998928"
---
# <a name="contactfolder-resource-type"></a><span data-ttu-id="8d1e3-103">contactFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="8d1e3-103">contactFolder resource type</span></span>

<span data-ttu-id="8d1e3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d1e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d1e3-105">包含联系人的文件夹。</span><span class="sxs-lookup"><span data-stu-id="8d1e3-105">A folder that contains contacts.</span></span>

<span data-ttu-id="8d1e3-106">该资源支持通过提供 [delta](../api/contactfolder-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="8d1e3-106">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contactfolder-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="8d1e3-107">方法</span><span class="sxs-lookup"><span data-stu-id="8d1e3-107">Methods</span></span>

| <span data-ttu-id="8d1e3-108">方法</span><span class="sxs-lookup"><span data-stu-id="8d1e3-108">Method</span></span>       | <span data-ttu-id="8d1e3-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="8d1e3-109">Return Type</span></span>  |<span data-ttu-id="8d1e3-110">说明</span><span class="sxs-lookup"><span data-stu-id="8d1e3-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8d1e3-111">获取 contactFolder</span><span class="sxs-lookup"><span data-stu-id="8d1e3-111">Get contactFolder</span></span>](../api/contactfolder-get.md) | [<span data-ttu-id="8d1e3-112">contactFolder</span><span class="sxs-lookup"><span data-stu-id="8d1e3-112">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="8d1e3-113">通过使用联系人文件夹 ID 获取联系人文件夹。</span><span class="sxs-lookup"><span data-stu-id="8d1e3-113">Get a contact folder by using the contact folder ID.</span></span>|
|[<span data-ttu-id="8d1e3-114">更新</span><span class="sxs-lookup"><span data-stu-id="8d1e3-114">Update</span></span>](../api/contactfolder-update.md) | [<span data-ttu-id="8d1e3-115">contactFolder</span><span class="sxs-lookup"><span data-stu-id="8d1e3-115">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="8d1e3-116">更新 contactFolder 对象。</span><span class="sxs-lookup"><span data-stu-id="8d1e3-116">Update contactFolder object.</span></span> |
|[<span data-ttu-id="8d1e3-117">删除</span><span class="sxs-lookup"><span data-stu-id="8d1e3-117">Delete</span></span>](../api/contactfolder-delete.md) | <span data-ttu-id="8d1e3-118">无</span><span class="sxs-lookup"><span data-stu-id="8d1e3-118">None</span></span> |<span data-ttu-id="8d1e3-119">删除 contactFolder 对象。</span><span class="sxs-lookup"><span data-stu-id="8d1e3-119">Delete contactFolder object.</span></span> |
|[<span data-ttu-id="8d1e3-120">列出 childFolder</span><span class="sxs-lookup"><span data-stu-id="8d1e3-120">List childFolders</span></span>](../api/contactfolder-list-childfolders.md) |<span data-ttu-id="8d1e3-121">[ContactFolder](contactfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8d1e3-121">[contactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="8d1e3-122">获取指定联系人文件夹下的子文件夹的集合。</span><span class="sxs-lookup"><span data-stu-id="8d1e3-122">Get a collection of child folders under the specified contact folder.</span></span>|
|[<span data-ttu-id="8d1e3-123">创建子 ContactFolder</span><span class="sxs-lookup"><span data-stu-id="8d1e3-123">Create child contactFolder</span></span>](../api/contactfolder-post-childfolders.md) |[<span data-ttu-id="8d1e3-124">contactFolder</span><span class="sxs-lookup"><span data-stu-id="8d1e3-124">contactFolder</span></span>](contactfolder.md)| <span data-ttu-id="8d1e3-125">创建新的 contactFolder 作为指定文件夹的子文件夹。</span><span class="sxs-lookup"><span data-stu-id="8d1e3-125">Create a new contactFolder as a child of a specified folder.</span></span>|
|[<span data-ttu-id="8d1e3-126">delta</span><span class="sxs-lookup"><span data-stu-id="8d1e3-126">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="8d1e3-127">[联系人](contact.md)集合</span><span class="sxs-lookup"><span data-stu-id="8d1e3-127">[contact](contact.md) collection</span></span>| <span data-ttu-id="8d1e3-128">获取用户邮箱中已添加、删除或移除的联系人文件夹集。</span><span class="sxs-lookup"><span data-stu-id="8d1e3-128">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="8d1e3-129">列出文件夹中的联系人</span><span class="sxs-lookup"><span data-stu-id="8d1e3-129">List contacts in folder</span></span>](../api/contactfolder-list-contacts.md) |<span data-ttu-id="8d1e3-130">[contact](contact.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8d1e3-130">[contact](contact.md) collection</span></span>| <span data-ttu-id="8d1e3-131">从已登录用户的默认联系人文件夹 (`.../me/contacts`) 或指定的联系人文件夹中获取联系人集合。</span><span class="sxs-lookup"><span data-stu-id="8d1e3-131">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>|
|[<span data-ttu-id="8d1e3-132">在文件夹中创建联系人</span><span class="sxs-lookup"><span data-stu-id="8d1e3-132">Create contact in folder</span></span>](../api/contactfolder-post-contacts.md) |[<span data-ttu-id="8d1e3-133">联系人</span><span class="sxs-lookup"><span data-stu-id="8d1e3-133">contact</span></span>](contact.md)| <span data-ttu-id="8d1e3-134">将联系人添加到联系人根文件夹或其他联系人文件夹的 `contacts` 终结点中。</span><span class="sxs-lookup"><span data-stu-id="8d1e3-134">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>|
|<span data-ttu-id="8d1e3-135">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="8d1e3-135">**Extended properties**</span></span>| | |
|[<span data-ttu-id="8d1e3-136">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="8d1e3-136">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="8d1e3-137">contactFolder</span><span class="sxs-lookup"><span data-stu-id="8d1e3-137">contactFolder</span></span>](contactfolder.md)  |<span data-ttu-id="8d1e3-138">在新建或现有的 contactFolder 中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="8d1e3-138">Create one or more single-value extended properties in a new or existing contactFolder.</span></span>   |
|[<span data-ttu-id="8d1e3-139">获取包含单值扩展属性的 contactFolder</span><span class="sxs-lookup"><span data-stu-id="8d1e3-139">Get contactFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="8d1e3-140">contactFolder</span><span class="sxs-lookup"><span data-stu-id="8d1e3-140">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="8d1e3-141">通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的 contactFolder。</span><span class="sxs-lookup"><span data-stu-id="8d1e3-141">Get contactFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="8d1e3-142">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="8d1e3-142">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="8d1e3-143">contactFolder</span><span class="sxs-lookup"><span data-stu-id="8d1e3-143">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="8d1e3-144">在新建或现有的 contactFolder 创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="8d1e3-144">Create one or more multi-value extended properties in a new or existing contactFolder.</span></span>  |
|[<span data-ttu-id="8d1e3-145">获取包含多值扩展属性的 contactFolder</span><span class="sxs-lookup"><span data-stu-id="8d1e3-145">Get contactFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="8d1e3-146">contactFolder</span><span class="sxs-lookup"><span data-stu-id="8d1e3-146">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="8d1e3-147">使用 `$expand` 获取包含一个多值扩展属性的 contactFolder。</span><span class="sxs-lookup"><span data-stu-id="8d1e3-147">Get a contactFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="8d1e3-148">属性</span><span class="sxs-lookup"><span data-stu-id="8d1e3-148">Properties</span></span>
| <span data-ttu-id="8d1e3-149">属性</span><span class="sxs-lookup"><span data-stu-id="8d1e3-149">Property</span></span>     | <span data-ttu-id="8d1e3-150">类型</span><span class="sxs-lookup"><span data-stu-id="8d1e3-150">Type</span></span>   |<span data-ttu-id="8d1e3-151">说明</span><span class="sxs-lookup"><span data-stu-id="8d1e3-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d1e3-152">displayName</span><span class="sxs-lookup"><span data-stu-id="8d1e3-152">displayName</span></span>|<span data-ttu-id="8d1e3-153">String</span><span class="sxs-lookup"><span data-stu-id="8d1e3-153">String</span></span>|<span data-ttu-id="8d1e3-154">文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="8d1e3-154">The folder's display name.</span></span>|
|<span data-ttu-id="8d1e3-155">id</span><span class="sxs-lookup"><span data-stu-id="8d1e3-155">id</span></span>|<span data-ttu-id="8d1e3-156">String</span><span class="sxs-lookup"><span data-stu-id="8d1e3-156">String</span></span>|<span data-ttu-id="8d1e3-p101">联系人文件夹的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="8d1e3-p101">Unique identifier of the contact folder. Read-only.</span></span>|
|<span data-ttu-id="8d1e3-159">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="8d1e3-159">parentFolderId</span></span>|<span data-ttu-id="8d1e3-160">String</span><span class="sxs-lookup"><span data-stu-id="8d1e3-160">String</span></span>|<span data-ttu-id="8d1e3-161">文件夹的父文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="8d1e3-161">The ID of the folder's parent folder.</span></span>|
|<span data-ttu-id="8d1e3-162">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="8d1e3-162">wellKnownName</span></span>|<span data-ttu-id="8d1e3-163">字符串</span><span class="sxs-lookup"><span data-stu-id="8d1e3-163">string</span></span>|<span data-ttu-id="8d1e3-164">文件夹的名称（如果文件夹是可识别的文件夹）。</span><span class="sxs-lookup"><span data-stu-id="8d1e3-164">The name of the folder if the folder is a recognized folder.</span></span> <span data-ttu-id="8d1e3-165">当前 `contacts` 是唯一可识别的 "联系人" 文件夹。</span><span class="sxs-lookup"><span data-stu-id="8d1e3-165">Currently `contacts` is the only recognized contacts folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d1e3-166">关系</span><span class="sxs-lookup"><span data-stu-id="8d1e3-166">Relationships</span></span>
| <span data-ttu-id="8d1e3-167">关系</span><span class="sxs-lookup"><span data-stu-id="8d1e3-167">Relationship</span></span> | <span data-ttu-id="8d1e3-168">类型</span><span class="sxs-lookup"><span data-stu-id="8d1e3-168">Type</span></span>   |<span data-ttu-id="8d1e3-169">说明</span><span class="sxs-lookup"><span data-stu-id="8d1e3-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d1e3-170">childFolders</span><span class="sxs-lookup"><span data-stu-id="8d1e3-170">childFolders</span></span>|<span data-ttu-id="8d1e3-171">[ContactFolder](contactfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8d1e3-171">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="8d1e3-p103">文件夹中的子文件夹集合。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="8d1e3-p103">The collection of child folders in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="8d1e3-176">contacts</span><span class="sxs-lookup"><span data-stu-id="8d1e3-176">contacts</span></span>|<span data-ttu-id="8d1e3-177">[Contact](contact.md) collection</span><span class="sxs-lookup"><span data-stu-id="8d1e3-177">[Contact](contact.md) collection</span></span>|<span data-ttu-id="8d1e3-p104">文件夹中的联系人。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="8d1e3-p104">The contacts in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="8d1e3-182">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="8d1e3-182">multiValueExtendedProperties</span></span>|<span data-ttu-id="8d1e3-183">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8d1e3-183">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="8d1e3-p105">为 contactFolder 定义的多值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="8d1e3-p105">The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="8d1e3-187">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="8d1e3-187">singleValueExtendedProperties</span></span>|<span data-ttu-id="8d1e3-188">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8d1e3-188">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="8d1e3-p106">为 contactFolder 定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="8d1e3-p106">The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8d1e3-192">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8d1e3-192">JSON representation</span></span>

<span data-ttu-id="8d1e3-193">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d1e3-193">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "contacts",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contactFolder"
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string",
  "wellKnownName": "string"
}

```

## <a name="see-also"></a><span data-ttu-id="8d1e3-194">另请参阅</span><span class="sxs-lookup"><span data-stu-id="8d1e3-194">See also</span></span>

- [<span data-ttu-id="8d1e3-195">使用增量查询跟踪 Microsoft Graph 数据更改</span><span class="sxs-lookup"><span data-stu-id="8d1e3-195">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="8d1e3-196">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="8d1e3-196">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


