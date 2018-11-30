---
title: contactFolder 资源类型
description: 包含联系人的文件夹。
ms.openlocfilehash: 3e9916d70a23c8acd4b1da2ee8f7e2df4c408e41
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045828"
---
# <a name="contactfolder-resource-type"></a><span data-ttu-id="90f5a-103">contactFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="90f5a-103">contactFolder resource type</span></span>

> <span data-ttu-id="90f5a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="90f5a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="90f5a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="90f5a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="90f5a-106">包含联系人的文件夹。</span><span class="sxs-lookup"><span data-stu-id="90f5a-106">A folder that contains contacts.</span></span>

<span data-ttu-id="90f5a-107">该资源支持通过提供 [delta](../api/contactfolder-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="90f5a-107">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contactfolder-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="90f5a-108">方法</span><span class="sxs-lookup"><span data-stu-id="90f5a-108">Methods</span></span>

| <span data-ttu-id="90f5a-109">方法</span><span class="sxs-lookup"><span data-stu-id="90f5a-109">Method</span></span>       | <span data-ttu-id="90f5a-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="90f5a-110">Return Type</span></span>  |<span data-ttu-id="90f5a-111">说明</span><span class="sxs-lookup"><span data-stu-id="90f5a-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="90f5a-112">获取 contactFolder</span><span class="sxs-lookup"><span data-stu-id="90f5a-112">Get contactFolder</span></span>](../api/contactfolder-get.md) | [<span data-ttu-id="90f5a-113">contactFolder</span><span class="sxs-lookup"><span data-stu-id="90f5a-113">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="90f5a-114">通过使用联系人文件夹 ID 获取联系人文件夹。</span><span class="sxs-lookup"><span data-stu-id="90f5a-114">Get a contact folder by using the contact folder ID.</span></span>|
|[<span data-ttu-id="90f5a-115">更新</span><span class="sxs-lookup"><span data-stu-id="90f5a-115">Update</span></span>](../api/contactfolder-update.md) | [<span data-ttu-id="90f5a-116">contactFolder</span><span class="sxs-lookup"><span data-stu-id="90f5a-116">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="90f5a-117">更新 contactFolder 对象。</span><span class="sxs-lookup"><span data-stu-id="90f5a-117">Update contactFolder object.</span></span> |
|[<span data-ttu-id="90f5a-118">删除</span><span class="sxs-lookup"><span data-stu-id="90f5a-118">Delete</span></span>](../api/contactfolder-delete.md) | <span data-ttu-id="90f5a-119">无</span><span class="sxs-lookup"><span data-stu-id="90f5a-119">None</span></span> |<span data-ttu-id="90f5a-120">删除 contactFolder 对象。</span><span class="sxs-lookup"><span data-stu-id="90f5a-120">Delete contactFolder object.</span></span> |
|[<span data-ttu-id="90f5a-121">列出 childFolder</span><span class="sxs-lookup"><span data-stu-id="90f5a-121">List childFolders</span></span>](../api/contactfolder-list-childfolders.md) |<span data-ttu-id="90f5a-122">[contactFolder](contactfolder.md)集合</span><span class="sxs-lookup"><span data-stu-id="90f5a-122">[contactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="90f5a-123">获取指定联系人文件夹下的子文件夹的集合。</span><span class="sxs-lookup"><span data-stu-id="90f5a-123">Get a collection of child folders under the specified contact folder.</span></span>|
|[<span data-ttu-id="90f5a-124">创建子 ContactFolder</span><span class="sxs-lookup"><span data-stu-id="90f5a-124">Create child contactFolder</span></span>](../api/contactfolder-post-childfolders.md) |[<span data-ttu-id="90f5a-125">contactFolder</span><span class="sxs-lookup"><span data-stu-id="90f5a-125">contactFolder</span></span>](contactfolder.md)| <span data-ttu-id="90f5a-126">创建新的 contactFolder 作为指定文件夹的子文件夹。</span><span class="sxs-lookup"><span data-stu-id="90f5a-126">Create a new contactFolder as a child of a specified folder.</span></span>|
|[<span data-ttu-id="90f5a-127">delta</span><span class="sxs-lookup"><span data-stu-id="90f5a-127">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="90f5a-128">[联系人](contact.md)集合</span><span class="sxs-lookup"><span data-stu-id="90f5a-128">[contact](contact.md) collection</span></span>| <span data-ttu-id="90f5a-129">获取用户邮箱中已添加、删除或移除的联系人文件夹集。</span><span class="sxs-lookup"><span data-stu-id="90f5a-129">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="90f5a-130">列出文件夹中的联系人</span><span class="sxs-lookup"><span data-stu-id="90f5a-130">List contacts in folder</span></span>](../api/contactfolder-list-contacts.md) |<span data-ttu-id="90f5a-131">[联系人](contact.md)集合</span><span class="sxs-lookup"><span data-stu-id="90f5a-131">[contact](contact.md) collection</span></span>| <span data-ttu-id="90f5a-132">从已登录用户的默认联系人文件夹 (`.../me/contacts`) 或指定的联系人文件夹中获取联系人集合。</span><span class="sxs-lookup"><span data-stu-id="90f5a-132">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>|
|[<span data-ttu-id="90f5a-133">在文件夹中创建联系人</span><span class="sxs-lookup"><span data-stu-id="90f5a-133">Create contact in folder</span></span>](../api/contactfolder-post-contacts.md) |[<span data-ttu-id="90f5a-134">联系人</span><span class="sxs-lookup"><span data-stu-id="90f5a-134">contact</span></span>](contact.md)| <span data-ttu-id="90f5a-135">将联系人添加到联系人根文件夹或其他联系人文件夹的 `contacts` 终结点中。</span><span class="sxs-lookup"><span data-stu-id="90f5a-135">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>|
|<span data-ttu-id="90f5a-136">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="90f5a-136">**Extended properties**</span></span>| | |
|[<span data-ttu-id="90f5a-137">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="90f5a-137">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="90f5a-138">contactFolder</span><span class="sxs-lookup"><span data-stu-id="90f5a-138">contactFolder</span></span>](contactfolder.md)  |<span data-ttu-id="90f5a-139">在新建或现有的 contactFolder 中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="90f5a-139">Create one or more single-value extended properties in a new or existing contactFolder.</span></span>   |
|[<span data-ttu-id="90f5a-140">获取包含单值扩展属性的 contactFolder</span><span class="sxs-lookup"><span data-stu-id="90f5a-140">Get contactFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="90f5a-141">contactFolder</span><span class="sxs-lookup"><span data-stu-id="90f5a-141">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="90f5a-142">通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的 contactFolder。</span><span class="sxs-lookup"><span data-stu-id="90f5a-142">Get contactFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="90f5a-143">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="90f5a-143">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="90f5a-144">contactFolder</span><span class="sxs-lookup"><span data-stu-id="90f5a-144">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="90f5a-145">在新建或现有的 contactFolder 创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="90f5a-145">Create one or more multi-value extended properties in a new or existing contactFolder.</span></span>  |
|[<span data-ttu-id="90f5a-146">获取包含多值扩展属性的 contactFolder</span><span class="sxs-lookup"><span data-stu-id="90f5a-146">Get contactFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="90f5a-147">contactFolder</span><span class="sxs-lookup"><span data-stu-id="90f5a-147">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="90f5a-148">使用 `$expand` 获取包含一个多值扩展属性的 contactFolder。</span><span class="sxs-lookup"><span data-stu-id="90f5a-148">Get a contactFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="90f5a-149">属性</span><span class="sxs-lookup"><span data-stu-id="90f5a-149">Properties</span></span>
| <span data-ttu-id="90f5a-150">属性</span><span class="sxs-lookup"><span data-stu-id="90f5a-150">Property</span></span>     | <span data-ttu-id="90f5a-151">类型</span><span class="sxs-lookup"><span data-stu-id="90f5a-151">Type</span></span>   |<span data-ttu-id="90f5a-152">说明</span><span class="sxs-lookup"><span data-stu-id="90f5a-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90f5a-153">displayName</span><span class="sxs-lookup"><span data-stu-id="90f5a-153">displayName</span></span>|<span data-ttu-id="90f5a-154">String</span><span class="sxs-lookup"><span data-stu-id="90f5a-154">String</span></span>|<span data-ttu-id="90f5a-155">文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="90f5a-155">The folder's display name.</span></span>|
|<span data-ttu-id="90f5a-156">id</span><span class="sxs-lookup"><span data-stu-id="90f5a-156">id</span></span>|<span data-ttu-id="90f5a-157">String</span><span class="sxs-lookup"><span data-stu-id="90f5a-157">String</span></span>|<span data-ttu-id="90f5a-p102">联系人文件夹的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="90f5a-p102">Unique identifier of the contact folder. Read-only.</span></span>|
|<span data-ttu-id="90f5a-160">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="90f5a-160">parentFolderId</span></span>|<span data-ttu-id="90f5a-161">String</span><span class="sxs-lookup"><span data-stu-id="90f5a-161">String</span></span>|<span data-ttu-id="90f5a-162">文件夹的父文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="90f5a-162">The ID of the folder's parent folder.</span></span>|
|<span data-ttu-id="90f5a-163">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="90f5a-163">wellKnownName</span></span>|<span data-ttu-id="90f5a-164">string</span><span class="sxs-lookup"><span data-stu-id="90f5a-164">string</span></span>|<span data-ttu-id="90f5a-165">如果文件夹为识别的文件夹的文件夹的名称。</span><span class="sxs-lookup"><span data-stu-id="90f5a-165">The name of the folder if the folder is a recognized folder.</span></span> <span data-ttu-id="90f5a-166">当前`contacts`是仅识别联系人文件夹。</span><span class="sxs-lookup"><span data-stu-id="90f5a-166">Currently `contacts` is the only recognized contacts folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="90f5a-167">Relationships</span><span class="sxs-lookup"><span data-stu-id="90f5a-167">Relationships</span></span>
| <span data-ttu-id="90f5a-168">关系</span><span class="sxs-lookup"><span data-stu-id="90f5a-168">Relationship</span></span> | <span data-ttu-id="90f5a-169">类型</span><span class="sxs-lookup"><span data-stu-id="90f5a-169">Type</span></span>   |<span data-ttu-id="90f5a-170">说明</span><span class="sxs-lookup"><span data-stu-id="90f5a-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90f5a-171">childFolders</span><span class="sxs-lookup"><span data-stu-id="90f5a-171">childFolders</span></span>|<span data-ttu-id="90f5a-172">[ContactFolder](contactfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90f5a-172">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="90f5a-p104">文件夹中的子文件夹集合。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="90f5a-p104">The collection of child folders in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="90f5a-177">contacts</span><span class="sxs-lookup"><span data-stu-id="90f5a-177">contacts</span></span>|<span data-ttu-id="90f5a-178">[联系人](contact.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90f5a-178">[Contact](contact.md) collection</span></span>|<span data-ttu-id="90f5a-p105">文件夹中的联系人。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="90f5a-p105">The contacts in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="90f5a-183">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="90f5a-183">multiValueExtendedProperties</span></span>|<span data-ttu-id="90f5a-184">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90f5a-184">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="90f5a-p106">为 contactFolder 定义的多值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="90f5a-p106">The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="90f5a-188">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="90f5a-188">singleValueExtendedProperties</span></span>|<span data-ttu-id="90f5a-189">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90f5a-189">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="90f5a-p107">为 contactFolder 定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="90f5a-p107">The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="90f5a-193">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="90f5a-193">JSON representation</span></span>

<span data-ttu-id="90f5a-194">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90f5a-194">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="90f5a-195">另请参阅</span><span class="sxs-lookup"><span data-stu-id="90f5a-195">See also</span></span>

- [<span data-ttu-id="90f5a-196">使用增量查询跟踪 Microsoft Graph 数据更改</span><span class="sxs-lookup"><span data-stu-id="90f5a-196">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="90f5a-197">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="90f5a-197">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
