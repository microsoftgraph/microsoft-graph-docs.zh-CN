---
title: contactFolder 资源类型
description: 包含联系人的文件夹。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 599f1765b6305d2dc4d482ec035ee4b24eb5183a
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640866"
---
# <a name="contactfolder-resource-type"></a><span data-ttu-id="d7359-103">contactFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="d7359-103">contactFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7359-104">包含联系人的文件夹。</span><span class="sxs-lookup"><span data-stu-id="d7359-104">A folder that contains contacts.</span></span>

<span data-ttu-id="d7359-105">该资源支持通过提供 [delta](../api/contactfolder-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="d7359-105">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contactfolder-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="d7359-106">方法</span><span class="sxs-lookup"><span data-stu-id="d7359-106">Methods</span></span>

| <span data-ttu-id="d7359-107">方法</span><span class="sxs-lookup"><span data-stu-id="d7359-107">Method</span></span>       | <span data-ttu-id="d7359-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="d7359-108">Return Type</span></span>  |<span data-ttu-id="d7359-109">说明</span><span class="sxs-lookup"><span data-stu-id="d7359-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d7359-110">获取 contactFolder</span><span class="sxs-lookup"><span data-stu-id="d7359-110">Get contactFolder</span></span>](../api/contactfolder-get.md) | [<span data-ttu-id="d7359-111">contactFolder</span><span class="sxs-lookup"><span data-stu-id="d7359-111">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="d7359-112">通过使用联系人文件夹 ID 获取联系人文件夹。</span><span class="sxs-lookup"><span data-stu-id="d7359-112">Get a contact folder by using the contact folder ID.</span></span>|
|[<span data-ttu-id="d7359-113">更新</span><span class="sxs-lookup"><span data-stu-id="d7359-113">Update</span></span>](../api/contactfolder-update.md) | [<span data-ttu-id="d7359-114">contactFolder</span><span class="sxs-lookup"><span data-stu-id="d7359-114">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="d7359-115">更新 contactFolder 对象。</span><span class="sxs-lookup"><span data-stu-id="d7359-115">Update contactFolder object.</span></span> |
|[<span data-ttu-id="d7359-116">删除</span><span class="sxs-lookup"><span data-stu-id="d7359-116">Delete</span></span>](../api/contactfolder-delete.md) | <span data-ttu-id="d7359-117">无</span><span class="sxs-lookup"><span data-stu-id="d7359-117">None</span></span> |<span data-ttu-id="d7359-118">删除 contactFolder 对象。</span><span class="sxs-lookup"><span data-stu-id="d7359-118">Delete contactFolder object.</span></span> |
|[<span data-ttu-id="d7359-119">列出 childFolder</span><span class="sxs-lookup"><span data-stu-id="d7359-119">List childFolders</span></span>](../api/contactfolder-list-childfolders.md) |<span data-ttu-id="d7359-120">[ContactFolder](contactfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d7359-120">[contactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="d7359-121">获取指定联系人文件夹下的子文件夹的集合。</span><span class="sxs-lookup"><span data-stu-id="d7359-121">Get a collection of child folders under the specified contact folder.</span></span>|
|[<span data-ttu-id="d7359-122">创建子 ContactFolder</span><span class="sxs-lookup"><span data-stu-id="d7359-122">Create child contactFolder</span></span>](../api/contactfolder-post-childfolders.md) |[<span data-ttu-id="d7359-123">contactFolder</span><span class="sxs-lookup"><span data-stu-id="d7359-123">contactFolder</span></span>](contactfolder.md)| <span data-ttu-id="d7359-124">创建新的 contactFolder 作为指定文件夹的子文件夹。</span><span class="sxs-lookup"><span data-stu-id="d7359-124">Create a new contactFolder as a child of a specified folder.</span></span>|
|[<span data-ttu-id="d7359-125">delta</span><span class="sxs-lookup"><span data-stu-id="d7359-125">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="d7359-126">[联系人](contact.md)集合</span><span class="sxs-lookup"><span data-stu-id="d7359-126">[contact](contact.md) collection</span></span>| <span data-ttu-id="d7359-127">获取用户邮箱中已添加、删除或移除的联系人文件夹集。</span><span class="sxs-lookup"><span data-stu-id="d7359-127">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="d7359-128">列出文件夹中的联系人</span><span class="sxs-lookup"><span data-stu-id="d7359-128">List contacts in folder</span></span>](../api/contactfolder-list-contacts.md) |<span data-ttu-id="d7359-129">[contact](contact.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d7359-129">[contact](contact.md) collection</span></span>| <span data-ttu-id="d7359-130">从已登录用户的默认联系人文件夹 (`.../me/contacts`) 或指定的联系人文件夹中获取联系人集合。</span><span class="sxs-lookup"><span data-stu-id="d7359-130">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>|
|[<span data-ttu-id="d7359-131">在文件夹中创建联系人</span><span class="sxs-lookup"><span data-stu-id="d7359-131">Create contact in folder</span></span>](../api/contactfolder-post-contacts.md) |[<span data-ttu-id="d7359-132">联系人</span><span class="sxs-lookup"><span data-stu-id="d7359-132">contact</span></span>](contact.md)| <span data-ttu-id="d7359-133">将联系人添加到联系人根文件夹或其他联系人文件夹的 `contacts` 终结点中。</span><span class="sxs-lookup"><span data-stu-id="d7359-133">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>|
|<span data-ttu-id="d7359-134">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="d7359-134">**Extended properties**</span></span>| | |
|[<span data-ttu-id="d7359-135">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="d7359-135">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="d7359-136">contactFolder</span><span class="sxs-lookup"><span data-stu-id="d7359-136">contactFolder</span></span>](contactfolder.md)  |<span data-ttu-id="d7359-137">在新建或现有的 contactFolder 中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="d7359-137">Create one or more single-value extended properties in a new or existing contactFolder.</span></span>   |
|[<span data-ttu-id="d7359-138">获取包含单值扩展属性的 contactFolder</span><span class="sxs-lookup"><span data-stu-id="d7359-138">Get contactFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="d7359-139">contactFolder</span><span class="sxs-lookup"><span data-stu-id="d7359-139">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="d7359-140">通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的 contactFolder。</span><span class="sxs-lookup"><span data-stu-id="d7359-140">Get contactFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="d7359-141">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="d7359-141">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="d7359-142">contactFolder</span><span class="sxs-lookup"><span data-stu-id="d7359-142">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="d7359-143">在新建或现有的 contactFolder 创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="d7359-143">Create one or more multi-value extended properties in a new or existing contactFolder.</span></span>  |
|[<span data-ttu-id="d7359-144">获取包含多值扩展属性的 contactFolder</span><span class="sxs-lookup"><span data-stu-id="d7359-144">Get contactFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="d7359-145">contactFolder</span><span class="sxs-lookup"><span data-stu-id="d7359-145">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="d7359-146">使用 `$expand` 获取包含一个多值扩展属性的 contactFolder。</span><span class="sxs-lookup"><span data-stu-id="d7359-146">Get a contactFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="d7359-147">属性</span><span class="sxs-lookup"><span data-stu-id="d7359-147">Properties</span></span>
| <span data-ttu-id="d7359-148">属性</span><span class="sxs-lookup"><span data-stu-id="d7359-148">Property</span></span>     | <span data-ttu-id="d7359-149">类型</span><span class="sxs-lookup"><span data-stu-id="d7359-149">Type</span></span>   |<span data-ttu-id="d7359-150">说明</span><span class="sxs-lookup"><span data-stu-id="d7359-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7359-151">displayName</span><span class="sxs-lookup"><span data-stu-id="d7359-151">displayName</span></span>|<span data-ttu-id="d7359-152">String</span><span class="sxs-lookup"><span data-stu-id="d7359-152">String</span></span>|<span data-ttu-id="d7359-153">文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d7359-153">The folder's display name.</span></span>|
|<span data-ttu-id="d7359-154">id</span><span class="sxs-lookup"><span data-stu-id="d7359-154">id</span></span>|<span data-ttu-id="d7359-155">String</span><span class="sxs-lookup"><span data-stu-id="d7359-155">String</span></span>|<span data-ttu-id="d7359-p101">联系人文件夹的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="d7359-p101">Unique identifier of the contact folder. Read-only.</span></span>|
|<span data-ttu-id="d7359-158">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="d7359-158">parentFolderId</span></span>|<span data-ttu-id="d7359-159">String</span><span class="sxs-lookup"><span data-stu-id="d7359-159">String</span></span>|<span data-ttu-id="d7359-160">文件夹的父文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="d7359-160">The ID of the folder's parent folder.</span></span>|
|<span data-ttu-id="d7359-161">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="d7359-161">wellKnownName</span></span>|<span data-ttu-id="d7359-162">string</span><span class="sxs-lookup"><span data-stu-id="d7359-162">string</span></span>|<span data-ttu-id="d7359-163">如果文件夹为识别的文件夹的文件夹的名称。</span><span class="sxs-lookup"><span data-stu-id="d7359-163">The name of the folder if the folder is a recognized folder.</span></span> <span data-ttu-id="d7359-164">当前`contacts`是仅识别联系人文件夹。</span><span class="sxs-lookup"><span data-stu-id="d7359-164">Currently `contacts` is the only recognized contacts folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7359-165">关系</span><span class="sxs-lookup"><span data-stu-id="d7359-165">Relationships</span></span>
| <span data-ttu-id="d7359-166">关系</span><span class="sxs-lookup"><span data-stu-id="d7359-166">Relationship</span></span> | <span data-ttu-id="d7359-167">类型</span><span class="sxs-lookup"><span data-stu-id="d7359-167">Type</span></span>   |<span data-ttu-id="d7359-168">说明</span><span class="sxs-lookup"><span data-stu-id="d7359-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7359-169">childFolders</span><span class="sxs-lookup"><span data-stu-id="d7359-169">childFolders</span></span>|<span data-ttu-id="d7359-170">[ContactFolder](contactfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d7359-170">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="d7359-p103">文件夹中的子文件夹集合。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="d7359-p103">The collection of child folders in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="d7359-175">contacts</span><span class="sxs-lookup"><span data-stu-id="d7359-175">contacts</span></span>|<span data-ttu-id="d7359-176">[联系人](contact.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d7359-176">[Contact](contact.md) collection</span></span>|<span data-ttu-id="d7359-p104">文件夹中的联系人。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="d7359-p104">The contacts in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="d7359-181">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="d7359-181">multiValueExtendedProperties</span></span>|<span data-ttu-id="d7359-182">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d7359-182">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="d7359-p105">为 contactFolder 定义的多值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="d7359-p105">The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="d7359-186">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="d7359-186">singleValueExtendedProperties</span></span>|<span data-ttu-id="d7359-187">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d7359-187">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="d7359-p106">为 contactFolder 定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="d7359-p106">The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d7359-191">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d7359-191">JSON representation</span></span>

<span data-ttu-id="d7359-192">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7359-192">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="d7359-193">另请参阅</span><span class="sxs-lookup"><span data-stu-id="d7359-193">See also</span></span>

- [<span data-ttu-id="d7359-194">使用增量查询跟踪 Microsoft Graph 数据更改</span><span class="sxs-lookup"><span data-stu-id="d7359-194">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="d7359-195">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="d7359-195">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/contactfolder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
