---
title: mailSearchFolder 资源类型
description: MailSearchFolder 是虚拟文件夹中包含与指定的搜索条件匹配的所有电子邮件项目的用户的邮箱。 mailSearchFolder 继承 mailFolder。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 1ba9ce248071e3d806383b4cd7e7550c1e3aa145
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920910"
---
# <a name="mailsearchfolder-resource-type"></a><span data-ttu-id="93c03-104">mailSearchFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="93c03-104">mailSearchFolder resource type</span></span>

> <span data-ttu-id="93c03-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="93c03-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93c03-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="93c03-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="93c03-107">MailSearchFolder 是虚拟文件夹中包含与指定的搜索条件匹配的所有电子邮件项目的用户的邮箱。</span><span class="sxs-lookup"><span data-stu-id="93c03-107">A mailSearchFolder is a virtual folder in the user's mailbox that contains all the email items matching specified search criteria.</span></span> <span data-ttu-id="93c03-108">mailSearchFolder 继承[mailFolder](mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="93c03-108">mailSearchFolder inherits from [mailFolder](mailfolder.md).</span></span>

## <a name="methods"></a><span data-ttu-id="93c03-109">方法</span><span class="sxs-lookup"><span data-stu-id="93c03-109">Methods</span></span>

| <span data-ttu-id="93c03-110">方法</span><span class="sxs-lookup"><span data-stu-id="93c03-110">Method</span></span> | <span data-ttu-id="93c03-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="93c03-111">Return Type</span></span>  | <span data-ttu-id="93c03-112">说明</span><span class="sxs-lookup"><span data-stu-id="93c03-112">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="93c03-113">创建搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="93c03-113">Create a search folder</span></span>](../api/mailsearchfolder-post.md) | [<span data-ttu-id="93c03-114">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="93c03-114">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="93c03-115">此用户的邮箱中创建搜索文件夹。</span><span class="sxs-lookup"><span data-stu-id="93c03-115">Create a search folder in this user's mailbox.</span></span> |
| [<span data-ttu-id="93c03-116">列表搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="93c03-116">List search folders</span></span>](../api/mailfolder-list-childfolders.md) | <span data-ttu-id="93c03-117">[mailFolder](mailfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="93c03-117">[mailFolder](mailfolder.md) collection</span></span> | <span data-ttu-id="93c03-118">列出该用户的邮箱，包括搜索文件夹中的所有文件夹。</span><span class="sxs-lookup"><span data-stu-id="93c03-118">List all the folders in this user's mailbox, including search folders.</span></span> |
| [<span data-ttu-id="93c03-119">获取搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="93c03-119">Get a search folder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="93c03-120">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="93c03-120">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="93c03-121">获取指定的搜索文件夹。</span><span class="sxs-lookup"><span data-stu-id="93c03-121">Get the specified search folder.</span></span> |
| [<span data-ttu-id="93c03-122">更新搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="93c03-122">Update a search folder</span></span>](../api/mailsearchfolder-update.md) | [<span data-ttu-id="93c03-123">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="93c03-123">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="93c03-124">更新指定的搜索文件夹。</span><span class="sxs-lookup"><span data-stu-id="93c03-124">Update the specified search folder.</span></span> |
| [<span data-ttu-id="93c03-125">删除搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="93c03-125">Delete a search folder</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="93c03-126">无</span><span class="sxs-lookup"><span data-stu-id="93c03-126">None</span></span> | <span data-ttu-id="93c03-127">删除指定的搜索文件夹。</span><span class="sxs-lookup"><span data-stu-id="93c03-127">Delete the specified search folder.</span></span> |
| [<span data-ttu-id="93c03-128">列表中搜索文件夹的所有邮件</span><span class="sxs-lookup"><span data-stu-id="93c03-128">List all messages in a search folder</span></span>](../api/mailfolder-list-messages.md) | <span data-ttu-id="93c03-129">[邮件](message.md)集合</span><span class="sxs-lookup"><span data-stu-id="93c03-129">[message](message.md) collection</span></span> | <span data-ttu-id="93c03-130">列表中指定的搜索文件夹的所有邮件。</span><span class="sxs-lookup"><span data-stu-id="93c03-130">List all the messages in the specified search folder.</span></span> |

## <a name="properties"></a><span data-ttu-id="93c03-131">属性</span><span class="sxs-lookup"><span data-stu-id="93c03-131">Properties</span></span>

| <span data-ttu-id="93c03-132">属性</span><span class="sxs-lookup"><span data-stu-id="93c03-132">Property</span></span> | <span data-ttu-id="93c03-133">类型</span><span class="sxs-lookup"><span data-stu-id="93c03-133">Type</span></span> | <span data-ttu-id="93c03-134">说明</span><span class="sxs-lookup"><span data-stu-id="93c03-134">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="93c03-135">isSupported</span><span class="sxs-lookup"><span data-stu-id="93c03-135">isSupported</span></span> | <span data-ttu-id="93c03-136">布尔</span><span class="sxs-lookup"><span data-stu-id="93c03-136">Boolean</span></span> | <span data-ttu-id="93c03-137">指示搜索文件夹是否可编辑使用 REST Api。</span><span class="sxs-lookup"><span data-stu-id="93c03-137">Indicates whether a search folder is editable using REST APIs.</span></span> |
| <span data-ttu-id="93c03-138">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="93c03-138">includeNestedFolders</span></span> | <span data-ttu-id="93c03-139">布尔</span><span class="sxs-lookup"><span data-stu-id="93c03-139">Boolean</span></span> | <span data-ttu-id="93c03-140">指示应如何遍历的邮箱文件夹层次结构。</span><span class="sxs-lookup"><span data-stu-id="93c03-140">Indicates how the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="93c03-141">`true`意味着应为深入搜索完成时`false`意味着浅表搜索应改为完成。</span><span class="sxs-lookup"><span data-stu-id="93c03-141">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="93c03-142">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="93c03-142">sourceFolderIDs</span></span> | <span data-ttu-id="93c03-143">String 集合</span><span class="sxs-lookup"><span data-stu-id="93c03-143">String collection</span></span> | <span data-ttu-id="93c03-144">应 mined 邮箱文件夹。</span><span class="sxs-lookup"><span data-stu-id="93c03-144">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="93c03-145">filterQuery</span><span class="sxs-lookup"><span data-stu-id="93c03-145">filterQuery</span></span> | <span data-ttu-id="93c03-146">字符串</span><span class="sxs-lookup"><span data-stu-id="93c03-146">String</span></span> | <span data-ttu-id="93c03-147">要筛选的邮件的 OData 查询。</span><span class="sxs-lookup"><span data-stu-id="93c03-147">The OData query to filter the messages.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="93c03-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="93c03-148">JSON representation</span></span>

<span data-ttu-id="93c03-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="93c03-149">The following is a JSON representation of the resource.</span></span>

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
