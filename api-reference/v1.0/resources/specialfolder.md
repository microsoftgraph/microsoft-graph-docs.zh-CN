---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SpecialFolder
localization_priority: Normal
description: SpecialFolder 资源将与特殊文件夹相关的数据项分组到一个单一结构。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 767ac4c5ce8819290e9a47e3e3f4f4efd1a9d238
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533633"
---
# <a name="specialfolder-resource-type"></a><span data-ttu-id="ce95f-103">SpecialFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="ce95f-103">SpecialFolder resource type</span></span>

<span data-ttu-id="ce95f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce95f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ce95f-105">**SpecialFolder** 资源将与特殊文件夹相关的数据项分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="ce95f-105">The **SpecialFolder** resource groups special folder-related data items into a single structure.</span></span>

<span data-ttu-id="ce95f-106">如果 **DriveItem** 具有一个非 null **specialFolder** facet，则该项表示特殊（命名的）文件夹。</span><span class="sxs-lookup"><span data-stu-id="ce95f-106">If a **DriveItem** has a non-null **specialFolder** facet, the item represents a special (named) folder.</span></span>
<span data-ttu-id="ce95f-107">可直接通过 [special folders 集合](../api/drive-get-specialfolder.md) 访问特殊文件夹。</span><span class="sxs-lookup"><span data-stu-id="ce95f-107">Special folders can be accessed directly via the [special folders collection](../api/drive-get-specialfolder.md).</span></span>

<span data-ttu-id="ce95f-p102">特殊文件夹可提供简单别名，因此无需按路径查找（需要本地化）文件夹或通过 ID 引用文件夹来访问已知文件夹。如果特殊文件夹被重命名或移到驱动器中的其他位置，此语法将继续返回该文件夹。</span><span class="sxs-lookup"><span data-stu-id="ce95f-p102">Special folders provide simple aliases to access well-known folders without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to return that folder.</span></span>

<span data-ttu-id="ce95f-p103">应用程序第一次尝试向特殊文件夹中写入内容时，如果特殊文件夹不存在，系统会自动创建特殊文件夹。如果用户删除某个特殊文件夹，再次向其写入内容时会重新创建特殊文件夹。</span><span class="sxs-lookup"><span data-stu-id="ce95f-p103">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

<span data-ttu-id="ce95f-112">**注意：** 如果应用仅请求 **Files.Read** 范围，而请求特殊文件夹不存在，则响应将是 `403 Forbidden` 错误。</span><span class="sxs-lookup"><span data-stu-id="ce95f-112">**Note:** If your app has only requested **Files.Read** scope and requests a special folder that doesn't exist, the response will be a `403 Forbidden` error.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce95f-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ce95f-113">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.specialFolder"
}-->
```json
{
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="ce95f-114">属性</span><span class="sxs-lookup"><span data-stu-id="ce95f-114">Properties</span></span>

| <span data-ttu-id="ce95f-115">属性</span><span class="sxs-lookup"><span data-stu-id="ce95f-115">Property</span></span>  | <span data-ttu-id="ce95f-116">类型</span><span class="sxs-lookup"><span data-stu-id="ce95f-116">Type</span></span>   | <span data-ttu-id="ce95f-117">说明</span><span class="sxs-lookup"><span data-stu-id="ce95f-117">Description</span></span>                                                            |
|:----------|:-------|:-----------------------------------------------------------------------|
| <span data-ttu-id="ce95f-118">name</span><span class="sxs-lookup"><span data-stu-id="ce95f-118">name</span></span>      | <span data-ttu-id="ce95f-119">string</span><span class="sxs-lookup"><span data-stu-id="ce95f-119">string</span></span> | <span data-ttu-id="ce95f-120">此项在 `/drive/special` 集合中的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ce95f-120">The unique identifier for this item in the `/drive/special` collection</span></span> |

## <a name="special-folders"></a><span data-ttu-id="ce95f-121">特殊文件夹</span><span class="sxs-lookup"><span data-stu-id="ce95f-121">Special folders</span></span>

<span data-ttu-id="ce95f-122">以下是 OneDrive 个人版和 OneDrive for Business 中可用的特殊文件夹。</span><span class="sxs-lookup"><span data-stu-id="ce95f-122">Here are the special folders available in OneDrive Personal and OneDrive for Business.</span></span>

| <span data-ttu-id="ce95f-123">名称</span><span class="sxs-lookup"><span data-stu-id="ce95f-123">Name</span></span>        | <span data-ttu-id="ce95f-124">文件夹 ID</span><span class="sxs-lookup"><span data-stu-id="ce95f-124">Folder id</span></span>    | <span data-ttu-id="ce95f-125">说明</span><span class="sxs-lookup"><span data-stu-id="ce95f-125">Description</span></span>                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| <span data-ttu-id="ce95f-126">App Root</span><span class="sxs-lookup"><span data-stu-id="ce95f-126">App Root</span></span>    | `approot`    | <span data-ttu-id="ce95f-p104">应用程序的个人文件夹。通常位于 `/Apps/{Application Name}` 中</span><span class="sxs-lookup"><span data-stu-id="ce95f-p104">The application's personal folder. Usually in `/Apps/{Application Name}`</span></span> |
| <span data-ttu-id="ce95f-129">本机照片</span><span class="sxs-lookup"><span data-stu-id="ce95f-129">Camera Roll</span></span> | `cameraroll` | <span data-ttu-id="ce95f-p105">本机照片备份文件夹。不适用于 OneDrive for Business。</span><span class="sxs-lookup"><span data-stu-id="ce95f-p105">The Camera Roll Backup folder. Not available in OneDrive for Business.</span></span>   |
| <span data-ttu-id="ce95f-132">Documents</span><span class="sxs-lookup"><span data-stu-id="ce95f-132">Documents</span></span>   | `documents`  | <span data-ttu-id="ce95f-133">“文档”文件夹。</span><span class="sxs-lookup"><span data-stu-id="ce95f-133">The Documents folder.</span></span>                                                    |
| <span data-ttu-id="ce95f-134">音乐</span><span class="sxs-lookup"><span data-stu-id="ce95f-134">Music</span></span>       | `music`      | <span data-ttu-id="ce95f-p106">音乐文件夹。不适用于 OneDrive for Business。</span><span class="sxs-lookup"><span data-stu-id="ce95f-p106">The Music folder. Not available in OneDrive for Business.</span></span>                |
| <span data-ttu-id="ce95f-137">Photos</span><span class="sxs-lookup"><span data-stu-id="ce95f-137">Photos</span></span>      | `photos`     | <span data-ttu-id="ce95f-138">“照片”文件夹。</span><span class="sxs-lookup"><span data-stu-id="ce95f-138">The Photos folder.</span></span>                                                       |

## <a name="remarks"></a><span data-ttu-id="ce95f-139">注解</span><span class="sxs-lookup"><span data-stu-id="ce95f-139">Remarks</span></span> 

<span data-ttu-id="ce95f-140">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="ce95f-140">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The SpecialFolder facet provides information about folders accessible as special folders.",
  "keywords": "special folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SpecialFolder"
} -->
