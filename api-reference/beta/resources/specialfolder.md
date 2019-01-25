---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SpecialFolder
localization_priority: Normal
ms.openlocfilehash: 5b187b1b4ff7183739ed734256a2d4c9e9fa9af6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512183"
---
# <a name="specialfolder-resource-type"></a><span data-ttu-id="4d3d7-102">SpecialFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="4d3d7-102">SpecialFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d3d7-103">**SpecialFolder** 资源将与特殊文件夹相关的数据项分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="4d3d7-103">The **SpecialFolder** resource groups special folder-related data items into a single structure.</span></span>

<span data-ttu-id="4d3d7-104">如果 **DriveItem** 具有一个非 null **specialFolder** facet，则该项表示特殊（命名的）文件夹。</span><span class="sxs-lookup"><span data-stu-id="4d3d7-104">If a **DriveItem** has a non-null **specialFolder** facet, the item represents a special (named) folder.</span></span>
<span data-ttu-id="4d3d7-105">可直接通过 [special folders 集合](../api/drive-get-specialfolder.md) 访问特殊文件夹。</span><span class="sxs-lookup"><span data-stu-id="4d3d7-105">Special folders can be accessed directly via the [special folders collection](../api/drive-get-specialfolder.md).</span></span>

<span data-ttu-id="4d3d7-p102">特殊文件夹可提供简单别名，因此无需按路径查找（需要本地化）文件夹或通过 ID 引用文件夹来访问已知文件夹。如果特殊文件夹被重命名或移到驱动器中的其他位置，此语法将继续返回该文件夹。</span><span class="sxs-lookup"><span data-stu-id="4d3d7-p102">Special folders provide simple aliases to access well-known folders without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to return that folder.</span></span>

<span data-ttu-id="4d3d7-p103">应用程序第一次尝试向特殊文件夹中写入内容时，如果特殊文件夹不存在，系统会自动创建特殊文件夹。如果用户删除某个特殊文件夹，再次向其写入内容时会重新创建特殊文件夹。</span><span class="sxs-lookup"><span data-stu-id="4d3d7-p103">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

<span data-ttu-id="4d3d7-110">**注意：** 如果应用仅请求 **Files.Read** 范围，而请求特殊文件夹不存在，则响应将是 `403 Forbidden` 错误。</span><span class="sxs-lookup"><span data-stu-id="4d3d7-110">**Note:** If your app has only requested **Files.Read** scope and requests a special folder that doesn't exist, the response will be a `403 Forbidden` error.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d3d7-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4d3d7-111">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="4d3d7-112">属性</span><span class="sxs-lookup"><span data-stu-id="4d3d7-112">Properties</span></span>

| <span data-ttu-id="4d3d7-113">属性</span><span class="sxs-lookup"><span data-stu-id="4d3d7-113">Property</span></span>  | <span data-ttu-id="4d3d7-114">类型</span><span class="sxs-lookup"><span data-stu-id="4d3d7-114">Type</span></span>   | <span data-ttu-id="4d3d7-115">说明</span><span class="sxs-lookup"><span data-stu-id="4d3d7-115">Description</span></span>                                                            |
|:----------|:-------|:-----------------------------------------------------------------------|
| <span data-ttu-id="4d3d7-116">name</span><span class="sxs-lookup"><span data-stu-id="4d3d7-116">name</span></span>      | <span data-ttu-id="4d3d7-117">string</span><span class="sxs-lookup"><span data-stu-id="4d3d7-117">string</span></span> | <span data-ttu-id="4d3d7-118">此项在 `/drive/special` 集合中的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4d3d7-118">The unique identifier for this item in the `/drive/special` collection</span></span> |

## <a name="special-folders"></a><span data-ttu-id="4d3d7-119">特殊文件夹</span><span class="sxs-lookup"><span data-stu-id="4d3d7-119">Special folders</span></span>

<span data-ttu-id="4d3d7-120">以下是 OneDrive 个人版和 OneDrive for Business 中可用的特殊文件夹。</span><span class="sxs-lookup"><span data-stu-id="4d3d7-120">Here are the special folders available in OneDrive Personal and OneDrive for Business.</span></span>

| <span data-ttu-id="4d3d7-121">名称</span><span class="sxs-lookup"><span data-stu-id="4d3d7-121">Name</span></span>        | <span data-ttu-id="4d3d7-122">文件夹 ID</span><span class="sxs-lookup"><span data-stu-id="4d3d7-122">Folder id</span></span>    | <span data-ttu-id="4d3d7-123">说明</span><span class="sxs-lookup"><span data-stu-id="4d3d7-123">Description</span></span>                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| <span data-ttu-id="4d3d7-124">应用根目录</span><span class="sxs-lookup"><span data-stu-id="4d3d7-124">App Root</span></span>    | `approot`    | <span data-ttu-id="4d3d7-p104">应用程序的个人文件夹。通常位于 `/Apps/{Application Name}` 中</span><span class="sxs-lookup"><span data-stu-id="4d3d7-p104">The application's personal folder. Usually in `/Apps/{Application Name}`</span></span> |
| <span data-ttu-id="4d3d7-127">本机照片</span><span class="sxs-lookup"><span data-stu-id="4d3d7-127">Camera Roll</span></span> | `cameraroll` | <span data-ttu-id="4d3d7-p105">本机照片备份文件夹。不适用于 OneDrive for Business。</span><span class="sxs-lookup"><span data-stu-id="4d3d7-p105">The Camera Roll Backup folder. Not available in OneDrive for Business.</span></span>   |
| <span data-ttu-id="4d3d7-130">文档</span><span class="sxs-lookup"><span data-stu-id="4d3d7-130">Documents</span></span>   | `documents`  | <span data-ttu-id="4d3d7-131">文档文件夹。</span><span class="sxs-lookup"><span data-stu-id="4d3d7-131">The Documents folder.</span></span>                                                    |
| <span data-ttu-id="4d3d7-132">音乐</span><span class="sxs-lookup"><span data-stu-id="4d3d7-132">Music</span></span>       | `music`      | <span data-ttu-id="4d3d7-p106">音乐文件夹。不适用于 OneDrive for Business。</span><span class="sxs-lookup"><span data-stu-id="4d3d7-p106">The Music folder. Not available in OneDrive for Business.</span></span>                |
| <span data-ttu-id="4d3d7-135">照片</span><span class="sxs-lookup"><span data-stu-id="4d3d7-135">Photos</span></span>      | `photos`     | <span data-ttu-id="4d3d7-136">照片文件夹。</span><span class="sxs-lookup"><span data-stu-id="4d3d7-136">The Photos folder.</span></span>                                                       |

## <a name="remarks"></a><span data-ttu-id="4d3d7-137">注解</span><span class="sxs-lookup"><span data-stu-id="4d3d7-137">Remarks</span></span> 

<span data-ttu-id="4d3d7-138">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="4d3d7-138">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The SpecialFolder facet provides information about folders accessible as special folders.",
  "keywords": "special folder,item,facet",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/specialfolder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
