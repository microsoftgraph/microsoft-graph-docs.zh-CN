---
title: 在 Microsoft Graph 中使用文件
description: 可以使用 Microsoft Graph 创建一个跨 OneDrive、OneDrive for Business 和 SharePoint 文档库与文件连接的应用程序。
localization_priority: Priority
ms.prod: sharepoint
author: jewan-microsoft
doc_type: conceptualPageType
ms.openlocfilehash: 3931fb9a327f682765b3795adbe90c4398cb38d5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079107"
---
# <a name="working-with-files-in-microsoft-graph"></a><span data-ttu-id="7ae8c-103">在 Microsoft Graph 中使用文件</span><span class="sxs-lookup"><span data-stu-id="7ae8c-103">Working with files in Microsoft Graph</span></span>

<span data-ttu-id="7ae8c-104">可以使用 Microsoft Graph 创建一个跨 OneDrive、OneDrive for Business 和 SharePoint 文档库与文件连接的应用程序。</span><span class="sxs-lookup"><span data-stu-id="7ae8c-104">You can use Microsoft Graph to create an app that connects with files across OneDrive, OneDrive for Business, and SharePoint document libraries.</span></span>
<span data-ttu-id="7ae8c-105">通过Microsoft Graph，你可以使用存储在Microsoft 365中的文件构建各种体验，从简单的存储用户文档到复杂的文件共享场景均可。</span><span class="sxs-lookup"><span data-stu-id="7ae8c-105">With Microsoft Graph, you can build a variety of experiences with files stored in Microsoft 365, from simply storing user documents to complex file-sharing scenarios.</span></span>

<span data-ttu-id="7ae8c-106">Microsoft Graph 公开可用于文件的两个资源类型：</span><span class="sxs-lookup"><span data-stu-id="7ae8c-106">Microsoft Graph exposes two resource types for working with files:</span></span>

* <span data-ttu-id="7ae8c-107">[驱动器](drive.md) - 表示文件的逻辑容器，例如文档库或用户的 OneDrive。</span><span class="sxs-lookup"><span data-stu-id="7ae8c-107">[Drive](drive.md) - Represents a logical container of files, like a document library or a user's OneDrive.</span></span>
* <span data-ttu-id="7ae8c-108">[DriveItem](driveitem.md) - 表示驱动器中的项目，例如文档、照片、视频或文件夹。</span><span class="sxs-lookup"><span data-stu-id="7ae8c-108">[DriveItem](driveitem.md) - Represents an item within a drive, like a document, photo, video, or folder.</span></span>

<span data-ttu-id="7ae8c-p102">大部分与文件的交互通过与 **DriveItem** 资源的交互实现。以下是一个 DriveItem 资源示例：</span><span class="sxs-lookup"><span data-stu-id="7ae8c-p102">Most of the interaction with files occurs through interaction with **DriveItem** resources. The following is an example of a DriveItem resource:</span></span>

```json
{
  "@content.downloadUrl":"https://public-sn3302.files.1drv.com/y2pcT7OaUEExF7EHOlpTjCE55mIUoiX7H3sx1ff6I-nP35XUTBqZlnkh9FJhWb_pf9sZ7LEpEchvDznIbQig0hWBeidpwFkOqSKCwQylisarN6T0ecAeMvantizBUzM2PA1",
  "createdDateTime": "2016-09-16T03:37:04.72Z",
  "cTag": "aYzpENDY0OEYwNkM5MUQ5RDNEITU0OTI3LjI1Ng",
  "eTag": "aRDQ2NDhGMDZDOTFEOUQzRCE1NDkyNy4w",
  "id":"D4648F06C91D9D3D!54927",
  "lastModifiedBy": {
    "user": {
      "displayName": "Daron Spektor",
      "id": "d4648f06c91d9d3d"
    }
  },
  "name":"BritishShorthair.jpg",
  "size":35212,
  "image":{
    "height":398,
    "width":273
  },
  "file": {
    "hashes":{
      "sha1Hash":"wmgPQ6jrSeMX7JP1XmstQEGM2fc="
    }
  }
}
```

<span data-ttu-id="7ae8c-111">**驱动器** 和 **DriveItem** 资源通过三种不同的方式公开数据：</span><span class="sxs-lookup"><span data-stu-id="7ae8c-111">**Drive** and **DriveItem** resources expose data in three different ways:</span></span>

* <span data-ttu-id="7ae8c-112">_属性_（像 **id** 和 **name**）公开简单的值（字符串、数字、布尔值）。</span><span class="sxs-lookup"><span data-stu-id="7ae8c-112">_Properties_ (like **id** and **name**) expose simple values (strings, numbers, Booleans).</span></span>
* <span data-ttu-id="7ae8c-p103">_Facet_（像**文件**和**照片**）公开复杂的值。存在的**文件**或**文件夹** Facet 表示 **DriveItem** 的行为和属性。</span><span class="sxs-lookup"><span data-stu-id="7ae8c-p103">_Facets_ (like **file** and **photo**) expose complex values. The presence of **file** or **folder** facets indicates behaviors and properties of a **DriveItem**.</span></span>
* <span data-ttu-id="7ae8c-115">_引用_（像**子项**和**缩略图**）指向其他资源的集合。</span><span class="sxs-lookup"><span data-stu-id="7ae8c-115">_References_ (like **children** and **thumbnails**) point to collections of other resources.</span></span>

## <a name="commonly-accessed-resources"></a><span data-ttu-id="7ae8c-116">经常访问的资源</span><span class="sxs-lookup"><span data-stu-id="7ae8c-116">Commonly accessed resources</span></span>

<span data-ttu-id="7ae8c-117">文件交互的大多数 API 请求将使用以下其中一种基础资源来访问**驱动器**或 **DriveItem**。</span><span class="sxs-lookup"><span data-stu-id="7ae8c-117">Most API requests for file interactions will use one of these base resources to access a **Drive** or **DriveItem**.</span></span>

| <span data-ttu-id="7ae8c-118">路径</span><span class="sxs-lookup"><span data-stu-id="7ae8c-118">Path</span></span>                               | <span data-ttu-id="7ae8c-119">资源</span><span class="sxs-lookup"><span data-stu-id="7ae8c-119">Resource</span></span>
|------------------------------------|-----------------------------------------
| `/me/drive`                        | <span data-ttu-id="7ae8c-120">用户的 OneDrive</span><span class="sxs-lookup"><span data-stu-id="7ae8c-120">User's OneDrive</span></span>
| `/me/drives`                       | <span data-ttu-id="7ae8c-121">枚举用户可用的 OneDrive 资源。</span><span class="sxs-lookup"><span data-stu-id="7ae8c-121">Enumerate OneDrive resources available to the user.</span></span>
| `/drives/{drive-id}`               | <span data-ttu-id="7ae8c-122">通过驱动器 ID 访问特定**驱动器**。</span><span class="sxs-lookup"><span data-stu-id="7ae8c-122">Access a specific **Drive** by the drive's ID.</span></span>
| `/drives/{drive-id}/root/children` | <span data-ttu-id="7ae8c-123">枚举特定**驱动器**根目录中的 **DriveItem** 资源。</span><span class="sxs-lookup"><span data-stu-id="7ae8c-123">Enumerate the **DriveItem** resources in the root of a specific **Drive**.</span></span>
| `/me/drive/items/{item-id}`        | <span data-ttu-id="7ae8c-124">通过其唯一 ID 访问用户 OneDrive 中的 **DriveItem**。</span><span class="sxs-lookup"><span data-stu-id="7ae8c-124">Access a **DriveItem** in the user's OneDrive by its unique ID.</span></span>
| `/me/drive/special/{special-id}`   | <span data-ttu-id="7ae8c-125">通过其已知名称访问用户 OneDrive 中的特殊（命名）文件夹。</span><span class="sxs-lookup"><span data-stu-id="7ae8c-125">Access a special (named) folder in the user's OneDrive by its known name.</span></span>
| `/users/{user-id}/drive`           | <span data-ttu-id="7ae8c-126">通过使用用户的唯一标识符访问另一个用户的 OneDrive 。</span><span class="sxs-lookup"><span data-stu-id="7ae8c-126">Access another user's OneDrive by using the user's unique ID.</span></span>
| `/groups/{group-id}/drive`         | <span data-ttu-id="7ae8c-127">通过组的唯一 ID 访问组的默认文档库。</span><span class="sxs-lookup"><span data-stu-id="7ae8c-127">Access the default document library for a group by the group's unique ID.</span></span>
| `/shares/{share-id}`               | <span data-ttu-id="7ae8c-128">通过其 **sharedId** 或共享 URL 访问 **DriveItem**。</span><span class="sxs-lookup"><span data-stu-id="7ae8c-128">Access a **DriveItem** by its **sharedId** or sharing URL.</span></span>
| `/sites/{site-id}/drive`           | <span data-ttu-id="7ae8c-129">访问给定 [SharePoint][] [网站][]的默认**驱动器**（文档库）</span><span class="sxs-lookup"><span data-stu-id="7ae8c-129">Access the default **Drive** (document library) for the given [SharePoint][] [site][]</span></span>
| `/sites/{site-id}/drives`          | <span data-ttu-id="7ae8c-130">枚举给定 [SharePoint][] [网站][]下的**驱动器**（文档库）</span><span class="sxs-lookup"><span data-stu-id="7ae8c-130">Enumerate the **Drives** (document libraries) under the given [SharePoint][] [site][]</span></span>

<span data-ttu-id="7ae8c-p104">除了通过唯一 ID 在**驱动器**内查找 **DriveItem**，应用还可以通过已知资源中的相对路径查找 **DriveItem**。要使用路径进行查找，请使用冒号 (`:`) 字符对相对路径转义。此表提供了通过不同的方法使用冒号字符来按路径查找项目的示例。</span><span class="sxs-lookup"><span data-stu-id="7ae8c-p104">In addition to addressing a **DriveItem** within a **Drive** by unique ID, your app can also address a **DriveItem** by relative path from a known resource. To address using a path, the colon (`:`) character is used to escape the relative path. This table provides an example of different ways to use the colon character to address an item by path.</span></span>

| <span data-ttu-id="7ae8c-134">路径</span><span class="sxs-lookup"><span data-stu-id="7ae8c-134">Path</span></span> | <span data-ttu-id="7ae8c-135">资源</span><span class="sxs-lookup"><span data-stu-id="7ae8c-135">Resource</span></span> |
|---|---|
| `/me/drive/root:/path/to/file` | <span data-ttu-id="7ae8c-136">通过相对于用户的 OneDrive 根文件夹的路径访问 **DriveItem**。</span><span class="sxs-lookup"><span data-stu-id="7ae8c-136">Access a **DriveItem** by path relative to the user's OneDrive root folder.</span></span> |
| `/me/drive/items/{item-id}:/path/to/file` | <span data-ttu-id="7ae8c-137">通过相对于另一项的路径访问 **DriveItem**（具有**文件夹** facet 的 **DriveItem**）。</span><span class="sxs-lookup"><span data-stu-id="7ae8c-137">Access a **DriveItem** by path relative to another item (a **DriveItem** with a **folder** facet).</span></span> |
| `/me/drive/root:/path/to/folder:/children` | <span data-ttu-id="7ae8c-138">通过相对于用户的 OneDrive 根文件夹的路径列出 **DriveItem** 的子项。</span><span class="sxs-lookup"><span data-stu-id="7ae8c-138">List the children of a **DriveItem** by path relative to the root of the user's OneDrive.</span></span> |
| `/me/drive/items/{item-id}:/path/to/folder:/children` | <span data-ttu-id="7ae8c-139">按照相对于另一项的路径列出 **DriveItem** 的子项。</span><span class="sxs-lookup"><span data-stu-id="7ae8c-139">List the children of a **DriveItem** by path relative to another item.</span></span> |

## <a name="drive-resource"></a><span data-ttu-id="7ae8c-140">驱动器资源</span><span class="sxs-lookup"><span data-stu-id="7ae8c-140">Drive resource</span></span>

<span data-ttu-id="7ae8c-141">[驱动器资源](drive.md) 是用户的 OneDrive 或 [SharePoint][] 文档库内的顶级对象。</span><span class="sxs-lookup"><span data-stu-id="7ae8c-141">The [Drive resource](drive.md) is the top-level object within a user's OneDrive or a [SharePoint][] document library.</span></span>
<span data-ttu-id="7ae8c-142">几乎所有的文件操作都从查找特定驱动器资源开始。</span><span class="sxs-lookup"><span data-stu-id="7ae8c-142">Nearly all files operations will start by addressing a specific drive resource.</span></span>

<span data-ttu-id="7ae8c-143">可以通过驱动器的唯一 ID 或 [用户](user.md)、[组](group.md) 或组织的默认驱动器查找驱动器资源。 </span><span class="sxs-lookup"><span data-stu-id="7ae8c-143">A drive resource can be addressed either by the drive's unique ID or by the default drive for a [User](user.md), [Group](group.md), or organization.</span></span>

## <a name="driveitem-resource"></a><span data-ttu-id="7ae8c-144">DriveItem 资源</span><span class="sxs-lookup"><span data-stu-id="7ae8c-144">DriveItem resource</span></span>

<span data-ttu-id="7ae8c-p106">[DriveItems](driveitem.md) 是驱动器文件系统内的对象。访问方法有：使用 `/items/{item-id}` 语法通过其 **id** 访问，或使用 `/root:/path/to/item/` 语法通过其文件系统路径访问。</span><span class="sxs-lookup"><span data-stu-id="7ae8c-p106">[DriveItems](driveitem.md) are the objects inside a drive's file system. They can be accessed by their **id** by using `/items/{item-id}` syntax, or by their file system path using the `/root:/path/to/item/` syntax.</span></span>

<span data-ttu-id="7ae8c-147">DriveItems 拥有多个 _Facet_，可提供有关项目标识和功能的数据。</span><span class="sxs-lookup"><span data-stu-id="7ae8c-147">DriveItems have _facets_ that provide data about the item's identity and capabilities.</span></span>

<span data-ttu-id="7ae8c-148">具有**文件夹** Facet 的 DriveItem 充当项目的容器，并且具有指向文件夹下的项目集合的**子项**引用。</span><span class="sxs-lookup"><span data-stu-id="7ae8c-148">DriveItems with a **folder** facet act as containers of items, and have a **children** reference, which points to a collection of items under the folder.</span></span>

## <a name="shared-folders-and-remote-items"></a><span data-ttu-id="7ae8c-149">共享文件夹和远程项目</span><span class="sxs-lookup"><span data-stu-id="7ae8c-149">Shared folders and remote items</span></span>

<span data-ttu-id="7ae8c-p107">OneDrive 个人版用户可以向他们自己的 OneDrive 中添加其他驱动器的一个或多个共享项目。这些共享项目在具有 [remoteItem](remoteitem.md) facet 的**子项**集合中显示为 **DriveItem**。</span><span class="sxs-lookup"><span data-stu-id="7ae8c-p107">OneDrive personal users can add one or more shared items from another drive to their own OneDrive. These shared items appear as a **DriveItem** in the **children** collection with a [remoteItem](remoteitem.md) facet.</span></span>

<span data-ttu-id="7ae8c-152">有关使用共享文件夹和远程项目的详细信息，请参阅 [Remote items and shared folders](remoteitem.md)（远程项目和共享文件夹）。</span><span class="sxs-lookup"><span data-stu-id="7ae8c-152">For more information about working with shared folders and remote items, see [Remote items and shared folders](remoteitem.md).</span></span>

## <a name="sharing-and-permissions"></a><span data-ttu-id="7ae8c-153">共享和权限</span><span class="sxs-lookup"><span data-stu-id="7ae8c-153">Sharing and permissions</span></span>

<span data-ttu-id="7ae8c-p108">OneDrive 和 SharePoint 文档库最常见的操作之一是与其他人共享内容。Microsoft Graph 使你的应用程序可以创建 [共享链接](../api/driveitem-createlink.md)、[添加权限并发送邀请](../api/driveitem-invite.md) 到驱动器中的项目。</span><span class="sxs-lookup"><span data-stu-id="7ae8c-p108">One of the most common actions for OneDrive and SharePoint document libraries is sharing content with other people. Microsoft Graph allows your app to create [sharing links](../api/driveitem-createlink.md), [add permissions and send invitations](../api/driveitem-invite.md) to items in a drive.</span></span>

<span data-ttu-id="7ae8c-156">Microsoft Graph 还为应用提供了一种直接从共享链接 [访问共享内容](../api/shares-get.md) 的方法。</span><span class="sxs-lookup"><span data-stu-id="7ae8c-156">Microsoft Graph also provides a way for your app to [access shared content](../api/shares-get.md) directly from a sharing link.</span></span>

## <a name="whats-new"></a><span data-ttu-id="7ae8c-157">最近更新</span><span class="sxs-lookup"><span data-stu-id="7ae8c-157">What's new</span></span>
<span data-ttu-id="7ae8c-158">了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。</span><span class="sxs-lookup"><span data-stu-id="7ae8c-158">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

[SharePoint]: sharepoint.md
[网站]: site.md
[site]: site.md

