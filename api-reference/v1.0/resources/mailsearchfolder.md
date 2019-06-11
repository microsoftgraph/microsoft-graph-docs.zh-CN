---
title: mailSearchFolder 资源类型
description: MailSearchFolder 是用户邮箱中的虚拟文件夹, 其中包含与指定的搜索条件匹配的所有电子邮件项目。 mailSearchFolder 继承自 mailFolder。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 0980a99567a93b48c4bd75ef3510c51347d8d794
ms.sourcegitcommit: b742da101a3a232356bf748c42da3ba08a7539d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2019
ms.locfileid: "34818665"
---
# <a name="mailsearchfolder-resource-type"></a><span data-ttu-id="5f7a4-104">mailSearchFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="5f7a4-104">mailSearchFolder resource type</span></span>

<span data-ttu-id="5f7a4-105">**MailSearchFolder**是用户邮箱中的虚拟文件夹, 其中包含与指定的搜索条件匹配的所有电子邮件项目。</span><span class="sxs-lookup"><span data-stu-id="5f7a4-105">A **mailSearchFolder** is a virtual folder in the user's mailbox that contains all the email items matching specified search criteria.</span></span> <span data-ttu-id="5f7a4-106">**mailSearchFolder**继承自[mailFolder](mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="5f7a4-106">**mailSearchFolder** inherits from [mailFolder](mailfolder.md).</span></span> <span data-ttu-id="5f7a4-107">可以在用户的 Exchange Online 邮箱中的任何文件夹中创建搜索文件夹。</span><span class="sxs-lookup"><span data-stu-id="5f7a4-107">Search folders can be created in any folder in a user's Exchange Online mailbox.</span></span> <span data-ttu-id="5f7a4-108">但是, 在 Outlook 中显示的搜索文件夹、Outlook for web 或 Outlook Live 中, 必须在**WellKnownFolderName**文件夹中创建该文件夹。</span><span class="sxs-lookup"><span data-stu-id="5f7a4-108">However, for a search folder to appear in Outlook, Outlook for the web, or Outlook Live, the folder must be created in the **WellKnownFolderName.SearchFolders** folder.</span></span> 

## <a name="search-folder-lifecycle"></a><span data-ttu-id="5f7a4-109">搜索文件夹生命周期</span><span class="sxs-lookup"><span data-stu-id="5f7a4-109">Search folder lifecycle</span></span>

<span data-ttu-id="5f7a4-110">由于以下原因之一, Exchange Online 可以删除你的应用程序创建的搜索文件夹:</span><span class="sxs-lookup"><span data-stu-id="5f7a4-110">Search folders created by your application can be deleted by Exchange Online for one of the following reasons:</span></span>

1.  <span data-ttu-id="5f7a4-111">搜索文件夹在45天后过期 (不使用)。</span><span class="sxs-lookup"><span data-stu-id="5f7a4-111">Search folders expire after 45 days of no usage.</span></span> 
2.  <span data-ttu-id="5f7a4-112">可以为每个源文件夹创建的搜索文件夹的数量存在限制。</span><span class="sxs-lookup"><span data-stu-id="5f7a4-112">There are limits on the number of search folders that can be created per source folder.</span></span> <span data-ttu-id="5f7a4-113">当此限制被突破时, 将删除较旧的搜索文件夹, 以便为新的搜索文件夹。</span><span class="sxs-lookup"><span data-stu-id="5f7a4-113">When this limit is breached, older search folders are deleted to make way for new ones.</span></span> 

<span data-ttu-id="5f7a4-114">删除搜索文件夹时, 您的应用程序应创建一个新的 "搜索文件夹" 资源并使用相同的。</span><span class="sxs-lookup"><span data-stu-id="5f7a4-114">When a search folder is deleted, your app should create a new search folder resource and use the same.</span></span>


## <a name="methods"></a><span data-ttu-id="5f7a4-115">方法</span><span class="sxs-lookup"><span data-stu-id="5f7a4-115">Methods</span></span>

| <span data-ttu-id="5f7a4-116">方法</span><span class="sxs-lookup"><span data-stu-id="5f7a4-116">Method</span></span> | <span data-ttu-id="5f7a4-117">返回类型</span><span class="sxs-lookup"><span data-stu-id="5f7a4-117">Return Type</span></span>  | <span data-ttu-id="5f7a4-118">说明</span><span class="sxs-lookup"><span data-stu-id="5f7a4-118">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="5f7a4-119">创建搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="5f7a4-119">Create a search folder</span></span>](../api/mailsearchfolder-post.md) | [<span data-ttu-id="5f7a4-120">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="5f7a4-120">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="5f7a4-121">在此用户的邮箱中创建 "搜索文件夹"。</span><span class="sxs-lookup"><span data-stu-id="5f7a4-121">Create a search folder in this user's mailbox.</span></span> |
| [<span data-ttu-id="5f7a4-122">列出搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="5f7a4-122">List search folders</span></span>](../api/mailfolder-list-childfolders.md) | <span data-ttu-id="5f7a4-123">[mailFolder](mailfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5f7a4-123">[mailFolder](mailfolder.md) collection</span></span> | <span data-ttu-id="5f7a4-124">列出此用户的邮箱中的所有文件夹, 包括 "搜索文件夹"。</span><span class="sxs-lookup"><span data-stu-id="5f7a4-124">List all the folders in this user's mailbox, including search folders.</span></span> |
| [<span data-ttu-id="5f7a4-125">获取搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="5f7a4-125">Get a search folder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="5f7a4-126">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="5f7a4-126">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="5f7a4-127">获取指定的搜索文件夹。</span><span class="sxs-lookup"><span data-stu-id="5f7a4-127">Get the specified search folder.</span></span> |
| [<span data-ttu-id="5f7a4-128">更新搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="5f7a4-128">Update a search folder</span></span>](../api/mailsearchfolder-update.md) | [<span data-ttu-id="5f7a4-129">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="5f7a4-129">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="5f7a4-130">更新指定的搜索文件夹。</span><span class="sxs-lookup"><span data-stu-id="5f7a4-130">Update the specified search folder.</span></span> |
| [<span data-ttu-id="5f7a4-131">删除搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="5f7a4-131">Delete a search folder</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="5f7a4-132">无</span><span class="sxs-lookup"><span data-stu-id="5f7a4-132">None</span></span> | <span data-ttu-id="5f7a4-133">删除指定的搜索文件夹。</span><span class="sxs-lookup"><span data-stu-id="5f7a4-133">Delete the specified search folder.</span></span> |
| [<span data-ttu-id="5f7a4-134">列出搜索文件夹中的所有邮件</span><span class="sxs-lookup"><span data-stu-id="5f7a4-134">List all messages in a search folder</span></span>](../api/mailfolder-list-messages.md) | <span data-ttu-id="5f7a4-135">[message](message.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5f7a4-135">[message](message.md) collection</span></span> | <span data-ttu-id="5f7a4-136">列出指定的搜索文件夹中的所有邮件。</span><span class="sxs-lookup"><span data-stu-id="5f7a4-136">List all the messages in the specified search folder.</span></span> |

## <a name="properties"></a><span data-ttu-id="5f7a4-137">属性</span><span class="sxs-lookup"><span data-stu-id="5f7a4-137">Properties</span></span>

| <span data-ttu-id="5f7a4-138">属性</span><span class="sxs-lookup"><span data-stu-id="5f7a4-138">Property</span></span> | <span data-ttu-id="5f7a4-139">类型</span><span class="sxs-lookup"><span data-stu-id="5f7a4-139">Type</span></span> | <span data-ttu-id="5f7a4-140">说明</span><span class="sxs-lookup"><span data-stu-id="5f7a4-140">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="5f7a4-141">isSupported</span><span class="sxs-lookup"><span data-stu-id="5f7a4-141">isSupported</span></span> | <span data-ttu-id="5f7a4-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f7a4-142">Boolean</span></span> | <span data-ttu-id="5f7a4-143">指示是否可使用 REST Api 编辑搜索文件夹。</span><span class="sxs-lookup"><span data-stu-id="5f7a4-143">Indicates whether a search folder is editable using REST APIs.</span></span> |
| <span data-ttu-id="5f7a4-144">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="5f7a4-144">includeNestedFolders</span></span> | <span data-ttu-id="5f7a4-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f7a4-145">Boolean</span></span> | <span data-ttu-id="5f7a4-146">指示应如何在搜索中遍历邮箱文件夹层次结构。</span><span class="sxs-lookup"><span data-stu-id="5f7a4-146">Indicates how the mailbox folder hierarchy should be traversed in the search.</span></span> <span data-ttu-id="5f7a4-147">`true`表示应执行深入搜索以在**sourceFolderIds**中显式指定的每个文件夹的层次结构中包含子文件夹。</span><span class="sxs-lookup"><span data-stu-id="5f7a4-147">`true` means that a deep search should be done to include child folders in the hierarchy of each folder explicitly specified in **sourceFolderIds**.</span></span> <span data-ttu-id="5f7a4-148">`false`表示仅对**sourceFolderIds**中显式指定的每个文件夹进行浅表搜索。</span><span class="sxs-lookup"><span data-stu-id="5f7a4-148">`false` means a shallow search of only each of the folders explicitly specified in **sourceFolderIds**.</span></span> |
| <span data-ttu-id="5f7a4-149">sourceFolderIds</span><span class="sxs-lookup"><span data-stu-id="5f7a4-149">sourceFolderIds</span></span> | <span data-ttu-id="5f7a4-150">String collection</span><span class="sxs-lookup"><span data-stu-id="5f7a4-150">String collection</span></span> | <span data-ttu-id="5f7a4-151">应挖掘的邮箱文件夹。</span><span class="sxs-lookup"><span data-stu-id="5f7a4-151">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="5f7a4-152">filterQuery</span><span class="sxs-lookup"><span data-stu-id="5f7a4-152">filterQuery</span></span> | <span data-ttu-id="5f7a4-153">String</span><span class="sxs-lookup"><span data-stu-id="5f7a4-153">String</span></span> | <span data-ttu-id="5f7a4-154">用于筛选邮件的 OData 查询。</span><span class="sxs-lookup"><span data-stu-id="5f7a4-154">The OData query to filter the messages.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5f7a4-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5f7a4-155">JSON representation</span></span>

<span data-ttu-id="5f7a4-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f7a4-156">The following is a JSON representation of the resource.</span></span>

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
