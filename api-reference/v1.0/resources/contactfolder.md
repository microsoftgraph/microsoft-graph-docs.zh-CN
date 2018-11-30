---
title: contactFolder 资源类型
description: 包含联系人的文件夹。
ms.openlocfilehash: c9b3ab0a89c4786e8a5467fe8ce6309424d98398
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010262"
---
# <a name="contactfolder-resource-type"></a><span data-ttu-id="54aa0-103">contactFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="54aa0-103">contactFolder resource type</span></span>

<span data-ttu-id="54aa0-104">包含联系人的文件夹。</span><span class="sxs-lookup"><span data-stu-id="54aa0-104">A folder that contains contacts.</span></span>

<span data-ttu-id="54aa0-105">该资源支持通过提供 [delta](../api/contactfolder-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="54aa0-105">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contactfolder-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="54aa0-106">方法</span><span class="sxs-lookup"><span data-stu-id="54aa0-106">Methods</span></span>

| <span data-ttu-id="54aa0-107">方法</span><span class="sxs-lookup"><span data-stu-id="54aa0-107">Method</span></span>       | <span data-ttu-id="54aa0-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="54aa0-108">Return Type</span></span>  |<span data-ttu-id="54aa0-109">说明</span><span class="sxs-lookup"><span data-stu-id="54aa0-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="54aa0-110">获取 contactFolder</span><span class="sxs-lookup"><span data-stu-id="54aa0-110">Get contactFolder</span></span>](../api/contactfolder-get.md) | [<span data-ttu-id="54aa0-111">contactFolder</span><span class="sxs-lookup"><span data-stu-id="54aa0-111">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="54aa0-112">通过使用联系人文件夹 ID 获取联系人文件夹。</span><span class="sxs-lookup"><span data-stu-id="54aa0-112">Get a contact folder by using the contact folder ID.</span></span>|
|[<span data-ttu-id="54aa0-113">更新</span><span class="sxs-lookup"><span data-stu-id="54aa0-113">Update</span></span>](../api/contactfolder-update.md) | [<span data-ttu-id="54aa0-114">contactFolder</span><span class="sxs-lookup"><span data-stu-id="54aa0-114">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="54aa0-115">更新 contactFolder 对象。</span><span class="sxs-lookup"><span data-stu-id="54aa0-115">Update contactFolder object.</span></span> |
|[<span data-ttu-id="54aa0-116">删除</span><span class="sxs-lookup"><span data-stu-id="54aa0-116">Delete</span></span>](../api/contactfolder-delete.md) | <span data-ttu-id="54aa0-117">无</span><span class="sxs-lookup"><span data-stu-id="54aa0-117">None</span></span> |<span data-ttu-id="54aa0-118">删除 contactFolder 对象。</span><span class="sxs-lookup"><span data-stu-id="54aa0-118">Delete contactFolder object.</span></span> |
|[<span data-ttu-id="54aa0-119">列出 childFolder</span><span class="sxs-lookup"><span data-stu-id="54aa0-119">List childFolders</span></span>](../api/contactfolder-list-childfolders.md) |<span data-ttu-id="54aa0-120">[ContactFolder](contactfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="54aa0-120">[ContactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="54aa0-121">获取指定联系人文件夹下的子文件夹的集合。</span><span class="sxs-lookup"><span data-stu-id="54aa0-121">Get a collection of child folders under the specified contact folder.</span></span>|
|[<span data-ttu-id="54aa0-122">创建子 ContactFolder</span><span class="sxs-lookup"><span data-stu-id="54aa0-122">Create child contactFolder</span></span>](../api/contactfolder-post-childfolders.md) |[<span data-ttu-id="54aa0-123">ContactFolder</span><span class="sxs-lookup"><span data-stu-id="54aa0-123">ContactFolder</span></span>](contactfolder.md)| <span data-ttu-id="54aa0-124">创建新的 contactFolder 作为指定文件夹的子文件夹。</span><span class="sxs-lookup"><span data-stu-id="54aa0-124">Create a new contactFolder as a child of a specified folder.</span></span>|
|[<span data-ttu-id="54aa0-125">delta</span><span class="sxs-lookup"><span data-stu-id="54aa0-125">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="54aa0-126">[联系人](contact.md)集合</span><span class="sxs-lookup"><span data-stu-id="54aa0-126">[contact](contact.md) collection</span></span>| <span data-ttu-id="54aa0-127">获取用户邮箱中已添加、删除或移除的联系人文件夹集。</span><span class="sxs-lookup"><span data-stu-id="54aa0-127">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="54aa0-128">列出文件夹中的联系人</span><span class="sxs-lookup"><span data-stu-id="54aa0-128">List contacts in folder</span></span>](../api/contactfolder-list-contacts.md) |<span data-ttu-id="54aa0-129">[联系人](contact.md) 集合</span><span class="sxs-lookup"><span data-stu-id="54aa0-129">[Contact](contact.md) collection</span></span>| <span data-ttu-id="54aa0-130">从已登录用户的默认联系人文件夹 (`.../me/contacts`) 或指定的联系人文件夹中获取联系人集合。</span><span class="sxs-lookup"><span data-stu-id="54aa0-130">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>|
|[<span data-ttu-id="54aa0-131">在文件夹中创建联系人</span><span class="sxs-lookup"><span data-stu-id="54aa0-131">Create contact in folder</span></span>](../api/contactfolder-post-contacts.md) |[<span data-ttu-id="54aa0-132">联系人</span><span class="sxs-lookup"><span data-stu-id="54aa0-132">Contact</span></span>](contact.md)| <span data-ttu-id="54aa0-133">将联系人添加到联系人根文件夹或其他联系人文件夹的 `contacts` 端点中。</span><span class="sxs-lookup"><span data-stu-id="54aa0-133">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="54aa0-134">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="54aa0-134">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="54aa0-135">contactFolder</span><span class="sxs-lookup"><span data-stu-id="54aa0-135">contactFolder</span></span>](contactfolder.md)  |<span data-ttu-id="54aa0-136">在新建或现有的 contactFolder 中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="54aa0-136">Create one or more single-value extended properties in a new or existing contactFolder.</span></span>   |
|[<span data-ttu-id="54aa0-137">获取包含单值扩展属性的 contactFolder</span><span class="sxs-lookup"><span data-stu-id="54aa0-137">Get contactFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="54aa0-138">contactFolder</span><span class="sxs-lookup"><span data-stu-id="54aa0-138">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="54aa0-139">通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的 contactFolder。</span><span class="sxs-lookup"><span data-stu-id="54aa0-139">Get contactFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="54aa0-140">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="54aa0-140">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="54aa0-141">contactFolder</span><span class="sxs-lookup"><span data-stu-id="54aa0-141">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="54aa0-142">在新建或现有的 contactFolder 创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="54aa0-142">Create one or more multi-value extended properties in a new or existing contactFolder.</span></span>  |
|[<span data-ttu-id="54aa0-143">获取包含多值扩展属性的 contactFolder</span><span class="sxs-lookup"><span data-stu-id="54aa0-143">Get contactFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="54aa0-144">contactFolder</span><span class="sxs-lookup"><span data-stu-id="54aa0-144">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="54aa0-145">使用 `$expand` 获取包含一个多值扩展属性的 contactFolder。</span><span class="sxs-lookup"><span data-stu-id="54aa0-145">Get a contactFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="54aa0-146">属性</span><span class="sxs-lookup"><span data-stu-id="54aa0-146">Properties</span></span>
| <span data-ttu-id="54aa0-147">属性</span><span class="sxs-lookup"><span data-stu-id="54aa0-147">Property</span></span>     | <span data-ttu-id="54aa0-148">类型</span><span class="sxs-lookup"><span data-stu-id="54aa0-148">Type</span></span>   |<span data-ttu-id="54aa0-149">说明</span><span class="sxs-lookup"><span data-stu-id="54aa0-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="54aa0-150">displayName</span><span class="sxs-lookup"><span data-stu-id="54aa0-150">displayName</span></span>|<span data-ttu-id="54aa0-151">String</span><span class="sxs-lookup"><span data-stu-id="54aa0-151">String</span></span>|<span data-ttu-id="54aa0-152">文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="54aa0-152">The folder's display name.</span></span>|
|<span data-ttu-id="54aa0-153">id</span><span class="sxs-lookup"><span data-stu-id="54aa0-153">id</span></span>|<span data-ttu-id="54aa0-154">String</span><span class="sxs-lookup"><span data-stu-id="54aa0-154">String</span></span>|<span data-ttu-id="54aa0-p101">联系人文件夹的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="54aa0-p101">Unique identifier of the contact folder. Read-only.</span></span>|
|<span data-ttu-id="54aa0-157">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="54aa0-157">parentFolderId</span></span>|<span data-ttu-id="54aa0-158">String</span><span class="sxs-lookup"><span data-stu-id="54aa0-158">String</span></span>|<span data-ttu-id="54aa0-159">文件夹的父文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="54aa0-159">The ID of the folder's parent folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="54aa0-160">Relationships</span><span class="sxs-lookup"><span data-stu-id="54aa0-160">Relationships</span></span>
| <span data-ttu-id="54aa0-161">关系</span><span class="sxs-lookup"><span data-stu-id="54aa0-161">Relationship</span></span> | <span data-ttu-id="54aa0-162">类型</span><span class="sxs-lookup"><span data-stu-id="54aa0-162">Type</span></span>   |<span data-ttu-id="54aa0-163">说明</span><span class="sxs-lookup"><span data-stu-id="54aa0-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="54aa0-164">childFolders</span><span class="sxs-lookup"><span data-stu-id="54aa0-164">childFolders</span></span>|<span data-ttu-id="54aa0-165">[ContactFolder](contactfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="54aa0-165">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="54aa0-p102">文件夹中的子文件夹集合。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="54aa0-p102">The collection of child folders in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="54aa0-170">contacts</span><span class="sxs-lookup"><span data-stu-id="54aa0-170">contacts</span></span>|<span data-ttu-id="54aa0-171">[联系人](contact.md) 集合</span><span class="sxs-lookup"><span data-stu-id="54aa0-171">[Contact](contact.md) collection</span></span>|<span data-ttu-id="54aa0-p103">文件夹中的联系人。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="54aa0-p103">The contacts in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="54aa0-176">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="54aa0-176">multiValueExtendedProperties</span></span>|<span data-ttu-id="54aa0-177">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="54aa0-177">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="54aa0-p104">为 contactFolder 定义的多值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="54aa0-p104">The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="54aa0-181">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="54aa0-181">singleValueExtendedProperties</span></span>|<span data-ttu-id="54aa0-182">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="54aa0-182">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="54aa0-p105">为 contactFolder 定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="54aa0-p105">The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="54aa0-186">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="54aa0-186">JSON representation</span></span>

<span data-ttu-id="54aa0-187">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54aa0-187">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="54aa0-188">另请参阅</span><span class="sxs-lookup"><span data-stu-id="54aa0-188">See also</span></span>

- [<span data-ttu-id="54aa0-189">使用增量查询跟踪 Microsoft Graph 数据更改</span><span class="sxs-lookup"><span data-stu-id="54aa0-189">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="54aa0-190">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="54aa0-190">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
