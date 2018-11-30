---
title: mailSearchFolder 资源类型
description: MailSearchFolder 是虚拟文件夹中包含与指定的搜索条件匹配的所有电子邮件项目的用户的邮箱。 mailSearchFolder 继承 mailFolder。
ms.openlocfilehash: abce7c86e44fcee98042aecf753f0fdf4172365e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046540"
---
# <a name="mailsearchfolder-resource-type"></a><span data-ttu-id="bc6db-104">mailSearchFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="bc6db-104">mailSearchFolder resource type</span></span>

> <span data-ttu-id="bc6db-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bc6db-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc6db-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bc6db-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bc6db-107">MailSearchFolder 是虚拟文件夹中包含与指定的搜索条件匹配的所有电子邮件项目的用户的邮箱。</span><span class="sxs-lookup"><span data-stu-id="bc6db-107">A mailSearchFolder is a virtual folder in the user's mailbox that contains all the email items matching specified search criteria.</span></span> <span data-ttu-id="bc6db-108">mailSearchFolder 继承[mailFolder](mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="bc6db-108">mailSearchFolder inherits from [mailFolder](mailfolder.md).</span></span>

## <a name="methods"></a><span data-ttu-id="bc6db-109">方法</span><span class="sxs-lookup"><span data-stu-id="bc6db-109">Methods</span></span>

| <span data-ttu-id="bc6db-110">方法</span><span class="sxs-lookup"><span data-stu-id="bc6db-110">Method</span></span> | <span data-ttu-id="bc6db-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="bc6db-111">Return Type</span></span>  | <span data-ttu-id="bc6db-112">说明</span><span class="sxs-lookup"><span data-stu-id="bc6db-112">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="bc6db-113">创建搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="bc6db-113">Create a search folder</span></span>](../api/mailsearchfolder-post.md) | [<span data-ttu-id="bc6db-114">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="bc6db-114">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="bc6db-115">此用户的邮箱中创建搜索文件夹。</span><span class="sxs-lookup"><span data-stu-id="bc6db-115">Create a search folder in this user's mailbox.</span></span> |
| [<span data-ttu-id="bc6db-116">列表搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="bc6db-116">List search folders</span></span>](../api/mailfolder-list-childfolders.md) | <span data-ttu-id="bc6db-117">[mailFolder](mailfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bc6db-117">[mailFolder](mailfolder.md) collection</span></span> | <span data-ttu-id="bc6db-118">列出该用户的邮箱，包括搜索文件夹中的所有文件夹。</span><span class="sxs-lookup"><span data-stu-id="bc6db-118">List all the folders in this user's mailbox, including search folders.</span></span> |
| [<span data-ttu-id="bc6db-119">获取搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="bc6db-119">Get a search folder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="bc6db-120">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="bc6db-120">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="bc6db-121">获取指定的搜索文件夹。</span><span class="sxs-lookup"><span data-stu-id="bc6db-121">Get the specified search folder.</span></span> |
| [<span data-ttu-id="bc6db-122">更新搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="bc6db-122">Update a search folder</span></span>](../api/mailsearchfolder-update.md) | [<span data-ttu-id="bc6db-123">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="bc6db-123">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="bc6db-124">更新指定的搜索文件夹。</span><span class="sxs-lookup"><span data-stu-id="bc6db-124">Update the specified search folder.</span></span> |
| [<span data-ttu-id="bc6db-125">删除搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="bc6db-125">Delete a search folder</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="bc6db-126">无</span><span class="sxs-lookup"><span data-stu-id="bc6db-126">None</span></span> | <span data-ttu-id="bc6db-127">删除指定的搜索文件夹。</span><span class="sxs-lookup"><span data-stu-id="bc6db-127">Delete the specified search folder.</span></span> |
| [<span data-ttu-id="bc6db-128">列表中搜索文件夹的所有邮件</span><span class="sxs-lookup"><span data-stu-id="bc6db-128">List all messages in a search folder</span></span>](../api/mailfolder-list-messages.md) | <span data-ttu-id="bc6db-129">[邮件](message.md)集合</span><span class="sxs-lookup"><span data-stu-id="bc6db-129">[message](message.md) collection</span></span> | <span data-ttu-id="bc6db-130">列表中指定的搜索文件夹的所有邮件。</span><span class="sxs-lookup"><span data-stu-id="bc6db-130">List all the messages in the specified search folder.</span></span> |

## <a name="properties"></a><span data-ttu-id="bc6db-131">属性</span><span class="sxs-lookup"><span data-stu-id="bc6db-131">Properties</span></span>

| <span data-ttu-id="bc6db-132">属性</span><span class="sxs-lookup"><span data-stu-id="bc6db-132">Property</span></span> | <span data-ttu-id="bc6db-133">类型</span><span class="sxs-lookup"><span data-stu-id="bc6db-133">Type</span></span> | <span data-ttu-id="bc6db-134">说明</span><span class="sxs-lookup"><span data-stu-id="bc6db-134">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="bc6db-135">isSupported</span><span class="sxs-lookup"><span data-stu-id="bc6db-135">isSupported</span></span> | <span data-ttu-id="bc6db-136">布尔</span><span class="sxs-lookup"><span data-stu-id="bc6db-136">Boolean</span></span> | <span data-ttu-id="bc6db-137">指示搜索文件夹是否可编辑使用 REST Api。</span><span class="sxs-lookup"><span data-stu-id="bc6db-137">Indicates whether a search folder is editable using REST APIs.</span></span> |
| <span data-ttu-id="bc6db-138">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="bc6db-138">includeNestedFolders</span></span> | <span data-ttu-id="bc6db-139">布尔</span><span class="sxs-lookup"><span data-stu-id="bc6db-139">Boolean</span></span> | <span data-ttu-id="bc6db-140">指示应如何遍历的邮箱文件夹层次结构。</span><span class="sxs-lookup"><span data-stu-id="bc6db-140">Indicates how the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="bc6db-141">`true`意味着应为深入搜索完成时`false`意味着浅表搜索应改为完成。</span><span class="sxs-lookup"><span data-stu-id="bc6db-141">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="bc6db-142">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="bc6db-142">sourceFolderIDs</span></span> | <span data-ttu-id="bc6db-143">String 集合</span><span class="sxs-lookup"><span data-stu-id="bc6db-143">String collection</span></span> | <span data-ttu-id="bc6db-144">应 mined 邮箱文件夹。</span><span class="sxs-lookup"><span data-stu-id="bc6db-144">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="bc6db-145">filterQuery</span><span class="sxs-lookup"><span data-stu-id="bc6db-145">filterQuery</span></span> | <span data-ttu-id="bc6db-146">字符串</span><span class="sxs-lookup"><span data-stu-id="bc6db-146">String</span></span> | <span data-ttu-id="bc6db-147">要筛选的邮件的 OData 查询。</span><span class="sxs-lookup"><span data-stu-id="bc6db-147">The OData query to filter the messages.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bc6db-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bc6db-148">JSON representation</span></span>

<span data-ttu-id="bc6db-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc6db-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailSearchFolder"
}-->

```json
{
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIDs": ["string"],
  "filterQuery": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2018-01-23 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailSearchFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
