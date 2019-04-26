---
title: mailSearchFolder 资源类型
description: mailSearchFolder 是用户邮箱中的虚拟文件夹, 其中包含与指定的搜索条件匹配的所有电子邮件项目。 mailSearchFolder 继承自 mailFolder。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 15f334f2910c962c367242965bd2104c8f3edb79
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342743"
---
# <a name="mailsearchfolder-resource-type"></a><span data-ttu-id="163da-104">mailSearchFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="163da-104">mailSearchFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="163da-105">mailSearchFolder 是用户邮箱中的虚拟文件夹, 其中包含与指定的搜索条件匹配的所有电子邮件项目。</span><span class="sxs-lookup"><span data-stu-id="163da-105">A mailSearchFolder is a virtual folder in the user's mailbox that contains all the email items matching specified search criteria.</span></span> <span data-ttu-id="163da-106">mailSearchFolder 继承自[mailFolder](mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="163da-106">mailSearchFolder inherits from [mailFolder](mailfolder.md).</span></span>

## <a name="methods"></a><span data-ttu-id="163da-107">方法</span><span class="sxs-lookup"><span data-stu-id="163da-107">Methods</span></span>

| <span data-ttu-id="163da-108">方法</span><span class="sxs-lookup"><span data-stu-id="163da-108">Method</span></span> | <span data-ttu-id="163da-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="163da-109">Return Type</span></span>  | <span data-ttu-id="163da-110">说明</span><span class="sxs-lookup"><span data-stu-id="163da-110">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="163da-111">创建搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="163da-111">Create a search folder</span></span>](../api/mailsearchfolder-post.md) | [<span data-ttu-id="163da-112">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="163da-112">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="163da-113">在此用户的邮箱中创建 "搜索文件夹"。</span><span class="sxs-lookup"><span data-stu-id="163da-113">Create a search folder in this user's mailbox.</span></span> |
| [<span data-ttu-id="163da-114">列出搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="163da-114">List search folders</span></span>](../api/mailfolder-list-childfolders.md) | <span data-ttu-id="163da-115">[mailFolder](mailfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="163da-115">[mailFolder](mailfolder.md) collection</span></span> | <span data-ttu-id="163da-116">列出此用户的邮箱中的所有文件夹, 包括 "搜索文件夹"。</span><span class="sxs-lookup"><span data-stu-id="163da-116">List all the folders in this user's mailbox, including search folders.</span></span> |
| [<span data-ttu-id="163da-117">获取搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="163da-117">Get a search folder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="163da-118">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="163da-118">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="163da-119">获取指定的搜索文件夹。</span><span class="sxs-lookup"><span data-stu-id="163da-119">Get the specified search folder.</span></span> |
| [<span data-ttu-id="163da-120">更新搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="163da-120">Update a search folder</span></span>](../api/mailsearchfolder-update.md) | [<span data-ttu-id="163da-121">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="163da-121">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="163da-122">更新指定的搜索文件夹。</span><span class="sxs-lookup"><span data-stu-id="163da-122">Update the specified search folder.</span></span> |
| [<span data-ttu-id="163da-123">删除搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="163da-123">Delete a search folder</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="163da-124">无</span><span class="sxs-lookup"><span data-stu-id="163da-124">None</span></span> | <span data-ttu-id="163da-125">删除指定的搜索文件夹。</span><span class="sxs-lookup"><span data-stu-id="163da-125">Delete the specified search folder.</span></span> |
| [<span data-ttu-id="163da-126">列出搜索文件夹中的所有邮件</span><span class="sxs-lookup"><span data-stu-id="163da-126">List all messages in a search folder</span></span>](../api/mailfolder-list-messages.md) | <span data-ttu-id="163da-127">[邮件](message.md)集合</span><span class="sxs-lookup"><span data-stu-id="163da-127">[message](message.md) collection</span></span> | <span data-ttu-id="163da-128">列出指定的搜索文件夹中的所有邮件。</span><span class="sxs-lookup"><span data-stu-id="163da-128">List all the messages in the specified search folder.</span></span> |

## <a name="properties"></a><span data-ttu-id="163da-129">属性</span><span class="sxs-lookup"><span data-stu-id="163da-129">Properties</span></span>

| <span data-ttu-id="163da-130">属性</span><span class="sxs-lookup"><span data-stu-id="163da-130">Property</span></span> | <span data-ttu-id="163da-131">类型</span><span class="sxs-lookup"><span data-stu-id="163da-131">Type</span></span> | <span data-ttu-id="163da-132">说明</span><span class="sxs-lookup"><span data-stu-id="163da-132">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="163da-133">isSupported</span><span class="sxs-lookup"><span data-stu-id="163da-133">isSupported</span></span> | <span data-ttu-id="163da-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="163da-134">Boolean</span></span> | <span data-ttu-id="163da-135">指示是否可使用 REST api 编辑搜索文件夹。</span><span class="sxs-lookup"><span data-stu-id="163da-135">Indicates whether a search folder is editable using REST APIs.</span></span> |
| <span data-ttu-id="163da-136">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="163da-136">includeNestedFolders</span></span> | <span data-ttu-id="163da-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="163da-137">Boolean</span></span> | <span data-ttu-id="163da-138">指示应如何遍历邮箱文件夹层次结构。</span><span class="sxs-lookup"><span data-stu-id="163da-138">Indicates how the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="163da-139">`true`表示应执行深入搜索, 而不是`false`指应改为进行浅表搜索。</span><span class="sxs-lookup"><span data-stu-id="163da-139">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="163da-140">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="163da-140">sourceFolderIDs</span></span> | <span data-ttu-id="163da-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="163da-141">String collection</span></span> | <span data-ttu-id="163da-142">应挖掘的邮箱文件夹。</span><span class="sxs-lookup"><span data-stu-id="163da-142">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="163da-143">filterQuery</span><span class="sxs-lookup"><span data-stu-id="163da-143">filterQuery</span></span> | <span data-ttu-id="163da-144">String</span><span class="sxs-lookup"><span data-stu-id="163da-144">String</span></span> | <span data-ttu-id="163da-145">用于筛选邮件的 OData 查询。</span><span class="sxs-lookup"><span data-stu-id="163da-145">The OData query to filter the messages.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="163da-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="163da-146">JSON representation</span></span>

<span data-ttu-id="163da-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="163da-147">The following is a JSON representation of the resource.</span></span>

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
