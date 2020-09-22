---
title: contactFolder 资源类型
description: 包含联系人的文件夹。
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: e18c1688bced04f20d12211fb5e5a70e884bd0b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056975"
---
# <a name="contactfolder-resource-type"></a><span data-ttu-id="28632-103">contactFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="28632-103">contactFolder resource type</span></span>

<span data-ttu-id="28632-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28632-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="28632-105">包含联系人的文件夹。</span><span class="sxs-lookup"><span data-stu-id="28632-105">A folder that contains contacts.</span></span>

<span data-ttu-id="28632-106">该资源支持通过提供 [delta](../api/contactfolder-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="28632-106">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contactfolder-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="28632-107">方法</span><span class="sxs-lookup"><span data-stu-id="28632-107">Methods</span></span>

| <span data-ttu-id="28632-108">方法</span><span class="sxs-lookup"><span data-stu-id="28632-108">Method</span></span>       | <span data-ttu-id="28632-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="28632-109">Return Type</span></span>  |<span data-ttu-id="28632-110">说明</span><span class="sxs-lookup"><span data-stu-id="28632-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="28632-111">获取 contactFolder</span><span class="sxs-lookup"><span data-stu-id="28632-111">Get contactFolder</span></span>](../api/contactfolder-get.md) | [<span data-ttu-id="28632-112">contactFolder</span><span class="sxs-lookup"><span data-stu-id="28632-112">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="28632-113">通过使用联系人文件夹 ID 获取联系人文件夹。</span><span class="sxs-lookup"><span data-stu-id="28632-113">Get a contact folder by using the contact folder ID.</span></span>|
|[<span data-ttu-id="28632-114">更新</span><span class="sxs-lookup"><span data-stu-id="28632-114">Update</span></span>](../api/contactfolder-update.md) | [<span data-ttu-id="28632-115">contactFolder</span><span class="sxs-lookup"><span data-stu-id="28632-115">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="28632-116">更新 contactFolder 对象。</span><span class="sxs-lookup"><span data-stu-id="28632-116">Update contactFolder object.</span></span> |
|[<span data-ttu-id="28632-117">删除</span><span class="sxs-lookup"><span data-stu-id="28632-117">Delete</span></span>](../api/contactfolder-delete.md) | <span data-ttu-id="28632-118">无</span><span class="sxs-lookup"><span data-stu-id="28632-118">None</span></span> |<span data-ttu-id="28632-119">删除 contactFolder 对象。</span><span class="sxs-lookup"><span data-stu-id="28632-119">Delete contactFolder object.</span></span> |
|[<span data-ttu-id="28632-120">列出 childFolder</span><span class="sxs-lookup"><span data-stu-id="28632-120">List childFolders</span></span>](../api/contactfolder-list-childfolders.md) |<span data-ttu-id="28632-121">[ContactFolder](contactfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="28632-121">[ContactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="28632-122">获取指定联系人文件夹下的子文件夹的集合。</span><span class="sxs-lookup"><span data-stu-id="28632-122">Get a collection of child folders under the specified contact folder.</span></span>|
|[<span data-ttu-id="28632-123">创建子 ContactFolder</span><span class="sxs-lookup"><span data-stu-id="28632-123">Create child contactFolder</span></span>](../api/contactfolder-post-childfolders.md) |[<span data-ttu-id="28632-124">ContactFolder</span><span class="sxs-lookup"><span data-stu-id="28632-124">ContactFolder</span></span>](contactfolder.md)| <span data-ttu-id="28632-125">创建新的 contactFolder 作为指定文件夹的子文件夹。</span><span class="sxs-lookup"><span data-stu-id="28632-125">Create a new contactFolder as a child of a specified folder.</span></span>|
|[<span data-ttu-id="28632-126">delta</span><span class="sxs-lookup"><span data-stu-id="28632-126">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="28632-127">[联系人](contact.md)集合</span><span class="sxs-lookup"><span data-stu-id="28632-127">[contact](contact.md) collection</span></span>| <span data-ttu-id="28632-128">获取用户邮箱中已添加、删除或移除的联系人文件夹集。</span><span class="sxs-lookup"><span data-stu-id="28632-128">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="28632-129">列出文件夹中的联系人</span><span class="sxs-lookup"><span data-stu-id="28632-129">List contacts in folder</span></span>](../api/contactfolder-list-contacts.md) |<span data-ttu-id="28632-130">[联系人](contact.md) 集合</span><span class="sxs-lookup"><span data-stu-id="28632-130">[Contact](contact.md) collection</span></span>| <span data-ttu-id="28632-131">从已登录用户的默认联系人文件夹 (`.../me/contacts`) 或指定的联系人文件夹中获取联系人集合。</span><span class="sxs-lookup"><span data-stu-id="28632-131">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>|
|[<span data-ttu-id="28632-132">在文件夹中创建联系人</span><span class="sxs-lookup"><span data-stu-id="28632-132">Create contact in folder</span></span>](../api/contactfolder-post-contacts.md) |[<span data-ttu-id="28632-133">联系人</span><span class="sxs-lookup"><span data-stu-id="28632-133">Contact</span></span>](contact.md)| <span data-ttu-id="28632-134">将联系人添加到联系人根文件夹或其他联系人文件夹的 `contacts` 端点中。</span><span class="sxs-lookup"><span data-stu-id="28632-134">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="28632-135">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="28632-135">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="28632-136">contactFolder</span><span class="sxs-lookup"><span data-stu-id="28632-136">contactFolder</span></span>](contactfolder.md)  |<span data-ttu-id="28632-137">在新建或现有的 contactFolder 中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="28632-137">Create one or more single-value extended properties in a new or existing contactFolder.</span></span>   |
|[<span data-ttu-id="28632-138">获取包含单值扩展属性的 contactFolder</span><span class="sxs-lookup"><span data-stu-id="28632-138">Get contactFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="28632-139">contactFolder</span><span class="sxs-lookup"><span data-stu-id="28632-139">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="28632-140">通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的 contactFolder。</span><span class="sxs-lookup"><span data-stu-id="28632-140">Get contactFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="28632-141">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="28632-141">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="28632-142">contactFolder</span><span class="sxs-lookup"><span data-stu-id="28632-142">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="28632-143">在新建或现有的 contactFolder 创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="28632-143">Create one or more multi-value extended properties in a new or existing contactFolder.</span></span>  |
|[<span data-ttu-id="28632-144">获取包含多值扩展属性的 contactFolder</span><span class="sxs-lookup"><span data-stu-id="28632-144">Get contactFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="28632-145">contactFolder</span><span class="sxs-lookup"><span data-stu-id="28632-145">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="28632-146">使用 `$expand` 获取包含一个多值扩展属性的 contactFolder。</span><span class="sxs-lookup"><span data-stu-id="28632-146">Get a contactFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="28632-147">属性</span><span class="sxs-lookup"><span data-stu-id="28632-147">Properties</span></span>
| <span data-ttu-id="28632-148">属性</span><span class="sxs-lookup"><span data-stu-id="28632-148">Property</span></span>     | <span data-ttu-id="28632-149">类型</span><span class="sxs-lookup"><span data-stu-id="28632-149">Type</span></span>   |<span data-ttu-id="28632-150">说明</span><span class="sxs-lookup"><span data-stu-id="28632-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28632-151">displayName</span><span class="sxs-lookup"><span data-stu-id="28632-151">displayName</span></span>|<span data-ttu-id="28632-152">String</span><span class="sxs-lookup"><span data-stu-id="28632-152">String</span></span>|<span data-ttu-id="28632-153">文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="28632-153">The folder's display name.</span></span>|
|<span data-ttu-id="28632-154">id</span><span class="sxs-lookup"><span data-stu-id="28632-154">id</span></span>|<span data-ttu-id="28632-155">String</span><span class="sxs-lookup"><span data-stu-id="28632-155">String</span></span>|<span data-ttu-id="28632-p101">联系人文件夹的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="28632-p101">Unique identifier of the contact folder. Read-only.</span></span>|
|<span data-ttu-id="28632-158">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="28632-158">parentFolderId</span></span>|<span data-ttu-id="28632-159">String</span><span class="sxs-lookup"><span data-stu-id="28632-159">String</span></span>|<span data-ttu-id="28632-160">文件夹的父文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="28632-160">The ID of the folder's parent folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28632-161">关系</span><span class="sxs-lookup"><span data-stu-id="28632-161">Relationships</span></span>
| <span data-ttu-id="28632-162">关系</span><span class="sxs-lookup"><span data-stu-id="28632-162">Relationship</span></span> | <span data-ttu-id="28632-163">类型</span><span class="sxs-lookup"><span data-stu-id="28632-163">Type</span></span>   |<span data-ttu-id="28632-164">说明</span><span class="sxs-lookup"><span data-stu-id="28632-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28632-165">childFolders</span><span class="sxs-lookup"><span data-stu-id="28632-165">childFolders</span></span>|<span data-ttu-id="28632-166">[ContactFolder](contactfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="28632-166">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="28632-p102">文件夹中的子文件夹集合。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="28632-p102">The collection of child folders in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="28632-171">contacts</span><span class="sxs-lookup"><span data-stu-id="28632-171">contacts</span></span>|<span data-ttu-id="28632-172">[Contact](contact.md) collection</span><span class="sxs-lookup"><span data-stu-id="28632-172">[Contact](contact.md) collection</span></span>|<span data-ttu-id="28632-p103">文件夹中的联系人。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="28632-p103">The contacts in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="28632-177">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="28632-177">multiValueExtendedProperties</span></span>|<span data-ttu-id="28632-178">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="28632-178">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="28632-p104">为 contactFolder 定义的多值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="28632-p104">The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="28632-182">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="28632-182">singleValueExtendedProperties</span></span>|<span data-ttu-id="28632-183">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="28632-183">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="28632-p105">为 contactFolder 定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="28632-p105">The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="28632-187">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="28632-187">JSON representation</span></span>

<span data-ttu-id="28632-188">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28632-188">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "contacts",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.contactFolder",
  "@odata.annotations": [
    {
      "property": "childFolders",
      "capabilities": {
        "navigability": "single",
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "contacts",
      "capabilities": {
        "changeTracking": true,
        "navigability": "single",
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string"
}

```

## <a name="see-also"></a><span data-ttu-id="28632-189">另请参阅</span><span class="sxs-lookup"><span data-stu-id="28632-189">See also</span></span>

- [<span data-ttu-id="28632-190">使用增量查询跟踪 Microsoft Graph 数据更改</span><span class="sxs-lookup"><span data-stu-id="28632-190">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="28632-191">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="28632-191">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

