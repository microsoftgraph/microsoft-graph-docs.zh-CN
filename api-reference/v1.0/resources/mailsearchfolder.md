---
title: mailSearchFolder 资源类型
description: mailSearchFolder 是用户邮箱中的虚拟文件夹，其中包含符合指定搜索条件的所有电子邮件项目。 mailSearchFolder 继承自 mailFolder。
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 9e153999cfa647b2f8f13e350b3193b358b536cf
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129707"
---
# <a name="mailsearchfolder-resource-type"></a><span data-ttu-id="dfe24-104">mailSearchFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="dfe24-104">mailSearchFolder resource type</span></span>

<span data-ttu-id="dfe24-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfe24-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dfe24-106">**mailSearchFolder** 是用户邮箱中的虚拟文件夹，其中包含符合指定搜索条件的所有电子邮件项目。</span><span class="sxs-lookup"><span data-stu-id="dfe24-106">A **mailSearchFolder** is a virtual folder in the user's mailbox that contains all the email items matching specified search criteria.</span></span> <span data-ttu-id="dfe24-107">**mailSearchFolder** 继承自 [mailFolder](mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="dfe24-107">**mailSearchFolder** inherits from [mailFolder](mailfolder.md).</span></span> <span data-ttu-id="dfe24-108">可以在用户的 Exchange Online 邮箱的任何文件夹中创建搜索文件夹。</span><span class="sxs-lookup"><span data-stu-id="dfe24-108">Search folders can be created in any folder in a user's Exchange Online mailbox.</span></span> <span data-ttu-id="dfe24-109">但是，若要在 Outlook、Outlook 网页或 Outlook Live 中显示搜索文件夹，必须在 **WellKnownFolderName.SearchFolders** 文件夹中创建该文件夹。</span><span class="sxs-lookup"><span data-stu-id="dfe24-109">However, for a search folder to appear in Outlook, Outlook for the web, or Outlook Live, the folder must be created in the **WellKnownFolderName.SearchFolders** folder.</span></span> 

## <a name="search-folder-lifecycle"></a><span data-ttu-id="dfe24-110">搜索文件夹生命周期</span><span class="sxs-lookup"><span data-stu-id="dfe24-110">Search folder lifecycle</span></span>

<span data-ttu-id="dfe24-111">Exchange Online 可以删除由应用程序创建的搜索文件夹，原因如下：</span><span class="sxs-lookup"><span data-stu-id="dfe24-111">Search folders created by your application can be deleted by Exchange Online for one of the following reasons:</span></span>

1.  <span data-ttu-id="dfe24-112">搜索文件夹在 45 天未使用后过期。</span><span class="sxs-lookup"><span data-stu-id="dfe24-112">Search folders expire after 45 days of no usage.</span></span> 
2.  <span data-ttu-id="dfe24-113">每个源文件夹可创建的搜索文件夹数量有一些限制。</span><span class="sxs-lookup"><span data-stu-id="dfe24-113">There are limits on the number of search folders that can be created per source folder.</span></span> <span data-ttu-id="dfe24-114">如果超过此限制，将删除较旧的搜索文件夹，为新的搜索文件夹提供途径。</span><span class="sxs-lookup"><span data-stu-id="dfe24-114">When this limit is breached, older search folders are deleted to make way for new ones.</span></span> 

<span data-ttu-id="dfe24-115">删除搜索文件夹后，应用应创建新的搜索文件夹资源，并使用相同的资源。</span><span class="sxs-lookup"><span data-stu-id="dfe24-115">When a search folder is deleted, your app should create a new search folder resource and use the same.</span></span>


## <a name="methods"></a><span data-ttu-id="dfe24-116">Methods</span><span class="sxs-lookup"><span data-stu-id="dfe24-116">Methods</span></span>

| <span data-ttu-id="dfe24-117">方法</span><span class="sxs-lookup"><span data-stu-id="dfe24-117">Method</span></span> | <span data-ttu-id="dfe24-118">返回类型</span><span class="sxs-lookup"><span data-stu-id="dfe24-118">Return Type</span></span>  | <span data-ttu-id="dfe24-119">说明</span><span class="sxs-lookup"><span data-stu-id="dfe24-119">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="dfe24-120">创建搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="dfe24-120">Create a search folder</span></span>](../api/mailsearchfolder-post.md) | [<span data-ttu-id="dfe24-121">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="dfe24-121">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="dfe24-122">在此用户的邮箱中创建搜索文件夹。</span><span class="sxs-lookup"><span data-stu-id="dfe24-122">Create a search folder in this user's mailbox.</span></span> |
| [<span data-ttu-id="dfe24-123">列出搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="dfe24-123">List search folders</span></span>](../api/mailfolder-list-childfolders.md) | <span data-ttu-id="dfe24-124">[mailFolder](mailfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dfe24-124">[mailFolder](mailfolder.md) collection</span></span> | <span data-ttu-id="dfe24-125">列出此用户邮箱中所有文件夹，包括搜索文件夹。</span><span class="sxs-lookup"><span data-stu-id="dfe24-125">List all the folders in this user's mailbox, including search folders.</span></span> |
| [<span data-ttu-id="dfe24-126">获取搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="dfe24-126">Get a search folder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="dfe24-127">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="dfe24-127">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="dfe24-128">获取指定的搜索文件夹。</span><span class="sxs-lookup"><span data-stu-id="dfe24-128">Get the specified search folder.</span></span> |
| [<span data-ttu-id="dfe24-129">更新搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="dfe24-129">Update a search folder</span></span>](../api/mailsearchfolder-update.md) | [<span data-ttu-id="dfe24-130">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="dfe24-130">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="dfe24-131">更新指定的搜索文件夹。</span><span class="sxs-lookup"><span data-stu-id="dfe24-131">Update the specified search folder.</span></span> |
| [<span data-ttu-id="dfe24-132">删除搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="dfe24-132">Delete a search folder</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="dfe24-133">无</span><span class="sxs-lookup"><span data-stu-id="dfe24-133">None</span></span> | <span data-ttu-id="dfe24-134">删除指定的搜索文件夹。</span><span class="sxs-lookup"><span data-stu-id="dfe24-134">Delete the specified search folder.</span></span> |
| [<span data-ttu-id="dfe24-135">列出搜索文件夹中的所有邮件</span><span class="sxs-lookup"><span data-stu-id="dfe24-135">List all messages in a search folder</span></span>](../api/mailfolder-list-messages.md) | <span data-ttu-id="dfe24-136">[邮件](message.md)集合</span><span class="sxs-lookup"><span data-stu-id="dfe24-136">[message](message.md) collection</span></span> | <span data-ttu-id="dfe24-137">列出指定搜索文件夹中的所有邮件。</span><span class="sxs-lookup"><span data-stu-id="dfe24-137">List all the messages in the specified search folder.</span></span> |

## <a name="properties"></a><span data-ttu-id="dfe24-138">属性</span><span class="sxs-lookup"><span data-stu-id="dfe24-138">Properties</span></span>

| <span data-ttu-id="dfe24-139">属性</span><span class="sxs-lookup"><span data-stu-id="dfe24-139">Property</span></span> | <span data-ttu-id="dfe24-140">类型</span><span class="sxs-lookup"><span data-stu-id="dfe24-140">Type</span></span> | <span data-ttu-id="dfe24-141">说明</span><span class="sxs-lookup"><span data-stu-id="dfe24-141">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="dfe24-142">isSupported</span><span class="sxs-lookup"><span data-stu-id="dfe24-142">isSupported</span></span> | <span data-ttu-id="dfe24-143">布尔</span><span class="sxs-lookup"><span data-stu-id="dfe24-143">Boolean</span></span> | <span data-ttu-id="dfe24-144">指示搜索文件夹是否可以使用 REST API 进行编辑。</span><span class="sxs-lookup"><span data-stu-id="dfe24-144">Indicates whether a search folder is editable using REST APIs.</span></span> |
| <span data-ttu-id="dfe24-145">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="dfe24-145">includeNestedFolders</span></span> | <span data-ttu-id="dfe24-146">布尔</span><span class="sxs-lookup"><span data-stu-id="dfe24-146">Boolean</span></span> | <span data-ttu-id="dfe24-147">指示如何在搜索中遍历邮箱文件夹层次结构。</span><span class="sxs-lookup"><span data-stu-id="dfe24-147">Indicates how the mailbox folder hierarchy should be traversed in the search.</span></span> <span data-ttu-id="dfe24-148">`true` 意味着应执行深入搜索，以在 **sourceFolderIds** 中显式指定的每个文件夹的层次结构中包括子文件夹。</span><span class="sxs-lookup"><span data-stu-id="dfe24-148">`true` means that a deep search should be done to include child folders in the hierarchy of each folder explicitly specified in **sourceFolderIds**.</span></span> <span data-ttu-id="dfe24-149">`false` 表示仅对 **sourceFolderIds** 中显式指定的每个文件夹进行浅表搜索。</span><span class="sxs-lookup"><span data-stu-id="dfe24-149">`false` means a shallow search of only each of the folders explicitly specified in **sourceFolderIds**.</span></span> |
| <span data-ttu-id="dfe24-150">sourceFolderIds</span><span class="sxs-lookup"><span data-stu-id="dfe24-150">sourceFolderIds</span></span> | <span data-ttu-id="dfe24-151">String collection</span><span class="sxs-lookup"><span data-stu-id="dfe24-151">String collection</span></span> | <span data-ttu-id="dfe24-152">应缩小的邮箱文件夹。</span><span class="sxs-lookup"><span data-stu-id="dfe24-152">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="dfe24-153">filterQuery</span><span class="sxs-lookup"><span data-stu-id="dfe24-153">filterQuery</span></span> | <span data-ttu-id="dfe24-154">String</span><span class="sxs-lookup"><span data-stu-id="dfe24-154">String</span></span> | <span data-ttu-id="dfe24-155">用于筛选邮件的 OData 查询。</span><span class="sxs-lookup"><span data-stu-id="dfe24-155">The OData query to filter the messages.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dfe24-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dfe24-156">JSON representation</span></span>

<span data-ttu-id="dfe24-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dfe24-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailSearchFolder"
}-->

```json
{
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIds": ["string"],
  "filterQuery": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2018-01-23 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailSearchFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

