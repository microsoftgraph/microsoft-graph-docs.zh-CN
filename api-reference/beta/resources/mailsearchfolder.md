---
title: mailSearchFolder 资源类型
description: MailSearchFolder 是虚拟文件夹中包含与指定的搜索条件匹配的所有电子邮件项目的用户的邮箱。 mailSearchFolder 继承 mailFolder。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ba76029b69d91be39c9d63ca755e8a4603aec0b9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520982"
---
# <a name="mailsearchfolder-resource-type"></a><span data-ttu-id="02dc4-104">mailSearchFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="02dc4-104">mailSearchFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02dc4-105">MailSearchFolder 是虚拟文件夹中包含与指定的搜索条件匹配的所有电子邮件项目的用户的邮箱。</span><span class="sxs-lookup"><span data-stu-id="02dc4-105">A mailSearchFolder is a virtual folder in the user's mailbox that contains all the email items matching specified search criteria.</span></span> <span data-ttu-id="02dc4-106">mailSearchFolder 继承[mailFolder](mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="02dc4-106">mailSearchFolder inherits from [mailFolder](mailfolder.md).</span></span>

## <a name="methods"></a><span data-ttu-id="02dc4-107">方法</span><span class="sxs-lookup"><span data-stu-id="02dc4-107">Methods</span></span>

| <span data-ttu-id="02dc4-108">方法</span><span class="sxs-lookup"><span data-stu-id="02dc4-108">Method</span></span> | <span data-ttu-id="02dc4-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="02dc4-109">Return Type</span></span>  | <span data-ttu-id="02dc4-110">说明</span><span class="sxs-lookup"><span data-stu-id="02dc4-110">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="02dc4-111">创建搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="02dc4-111">Create a search folder</span></span>](../api/mailsearchfolder-post.md) | [<span data-ttu-id="02dc4-112">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="02dc4-112">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="02dc4-113">此用户的邮箱中创建搜索文件夹。</span><span class="sxs-lookup"><span data-stu-id="02dc4-113">Create a search folder in this user's mailbox.</span></span> |
| [<span data-ttu-id="02dc4-114">列表搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="02dc4-114">List search folders</span></span>](../api/mailfolder-list-childfolders.md) | <span data-ttu-id="02dc4-115">[mailFolder](mailfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="02dc4-115">[mailFolder](mailfolder.md) collection</span></span> | <span data-ttu-id="02dc4-116">列出该用户的邮箱，包括搜索文件夹中的所有文件夹。</span><span class="sxs-lookup"><span data-stu-id="02dc4-116">List all the folders in this user's mailbox, including search folders.</span></span> |
| [<span data-ttu-id="02dc4-117">获取搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="02dc4-117">Get a search folder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="02dc4-118">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="02dc4-118">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="02dc4-119">获取指定的搜索文件夹。</span><span class="sxs-lookup"><span data-stu-id="02dc4-119">Get the specified search folder.</span></span> |
| [<span data-ttu-id="02dc4-120">更新搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="02dc4-120">Update a search folder</span></span>](../api/mailsearchfolder-update.md) | [<span data-ttu-id="02dc4-121">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="02dc4-121">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="02dc4-122">更新指定的搜索文件夹。</span><span class="sxs-lookup"><span data-stu-id="02dc4-122">Update the specified search folder.</span></span> |
| [<span data-ttu-id="02dc4-123">删除搜索文件夹</span><span class="sxs-lookup"><span data-stu-id="02dc4-123">Delete a search folder</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="02dc4-124">无</span><span class="sxs-lookup"><span data-stu-id="02dc4-124">None</span></span> | <span data-ttu-id="02dc4-125">删除指定的搜索文件夹。</span><span class="sxs-lookup"><span data-stu-id="02dc4-125">Delete the specified search folder.</span></span> |
| [<span data-ttu-id="02dc4-126">列表中搜索文件夹的所有邮件</span><span class="sxs-lookup"><span data-stu-id="02dc4-126">List all messages in a search folder</span></span>](../api/mailfolder-list-messages.md) | <span data-ttu-id="02dc4-127">[message](message.md) 集合</span><span class="sxs-lookup"><span data-stu-id="02dc4-127">[message](message.md) collection</span></span> | <span data-ttu-id="02dc4-128">列表中指定的搜索文件夹的所有邮件。</span><span class="sxs-lookup"><span data-stu-id="02dc4-128">List all the messages in the specified search folder.</span></span> |

## <a name="properties"></a><span data-ttu-id="02dc4-129">属性</span><span class="sxs-lookup"><span data-stu-id="02dc4-129">Properties</span></span>

| <span data-ttu-id="02dc4-130">属性</span><span class="sxs-lookup"><span data-stu-id="02dc4-130">Property</span></span> | <span data-ttu-id="02dc4-131">类型</span><span class="sxs-lookup"><span data-stu-id="02dc4-131">Type</span></span> | <span data-ttu-id="02dc4-132">说明</span><span class="sxs-lookup"><span data-stu-id="02dc4-132">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="02dc4-133">isSupported</span><span class="sxs-lookup"><span data-stu-id="02dc4-133">isSupported</span></span> | <span data-ttu-id="02dc4-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="02dc4-134">Boolean</span></span> | <span data-ttu-id="02dc4-135">指示搜索文件夹是否可编辑使用 REST Api。</span><span class="sxs-lookup"><span data-stu-id="02dc4-135">Indicates whether a search folder is editable using REST APIs.</span></span> |
| <span data-ttu-id="02dc4-136">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="02dc4-136">includeNestedFolders</span></span> | <span data-ttu-id="02dc4-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="02dc4-137">Boolean</span></span> | <span data-ttu-id="02dc4-138">指示应如何遍历的邮箱文件夹层次结构。</span><span class="sxs-lookup"><span data-stu-id="02dc4-138">Indicates how the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="02dc4-139">`true`意味着应为深入搜索完成时`false`意味着浅表搜索应改为完成。</span><span class="sxs-lookup"><span data-stu-id="02dc4-139">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="02dc4-140">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="02dc4-140">sourceFolderIDs</span></span> | <span data-ttu-id="02dc4-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="02dc4-141">String collection</span></span> | <span data-ttu-id="02dc4-142">应 mined 邮箱文件夹。</span><span class="sxs-lookup"><span data-stu-id="02dc4-142">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="02dc4-143">filterQuery</span><span class="sxs-lookup"><span data-stu-id="02dc4-143">filterQuery</span></span> | <span data-ttu-id="02dc4-144">String</span><span class="sxs-lookup"><span data-stu-id="02dc4-144">String</span></span> | <span data-ttu-id="02dc4-145">要筛选的邮件的 OData 查询。</span><span class="sxs-lookup"><span data-stu-id="02dc4-145">The OData query to filter the messages.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="02dc4-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="02dc4-146">JSON representation</span></span>

<span data-ttu-id="02dc4-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="02dc4-147">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/mailsearchfolder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
