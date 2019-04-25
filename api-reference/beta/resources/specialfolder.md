---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SpecialFolder
localization_priority: Normal
ms.openlocfilehash: ff1bee4ce71bf76c94951d298f80db74609710e6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582274"
---
# <a name="specialfolder-resource-type"></a><span data-ttu-id="14d64-102">SpecialFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="14d64-102">SpecialFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14d64-103">**SpecialFolder** 资源将与特殊文件夹相关的数据项分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="14d64-103">The **SpecialFolder** resource groups special folder-related data items into a single structure.</span></span>

<span data-ttu-id="14d64-104">如果 **DriveItem** 具有一个非 null **specialFolder** facet，则该项表示特殊（命名的）文件夹。</span><span class="sxs-lookup"><span data-stu-id="14d64-104">If a **DriveItem** has a non-null **specialFolder** facet, the item represents a special (named) folder.</span></span>
<span data-ttu-id="14d64-105">可直接通过 [special folders 集合](../api/drive-get-specialfolder.md) 访问特殊文件夹。</span><span class="sxs-lookup"><span data-stu-id="14d64-105">Special folders can be accessed directly via the [special folders collection](../api/drive-get-specialfolder.md).</span></span>

<span data-ttu-id="14d64-p102">特殊文件夹可提供简单别名，因此无需按路径查找（需要本地化）文件夹或通过 ID 引用文件夹来访问已知文件夹。如果特殊文件夹被重命名或移到驱动器中的其他位置，此语法将继续返回该文件夹。</span><span class="sxs-lookup"><span data-stu-id="14d64-p102">Special folders provide simple aliases to access well-known folders without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to return that folder.</span></span>

<span data-ttu-id="14d64-p103">应用程序第一次尝试向特殊文件夹中写入内容时，如果特殊文件夹不存在，系统会自动创建特殊文件夹。如果用户删除某个特殊文件夹，再次向其写入内容时会重新创建特殊文件夹。</span><span class="sxs-lookup"><span data-stu-id="14d64-p103">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

<span data-ttu-id="14d64-110">**注意：** 如果应用仅请求 **Files.Read** 范围，而请求特殊文件夹不存在，则响应将是 `403 Forbidden` 错误。</span><span class="sxs-lookup"><span data-stu-id="14d64-110">**Note:** If your app has only requested **Files.Read** scope and requests a special folder that doesn't exist, the response will be a `403 Forbidden` error.</span></span>

## <a name="json-representation"></a><span data-ttu-id="14d64-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="14d64-111">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="14d64-112">属性</span><span class="sxs-lookup"><span data-stu-id="14d64-112">Properties</span></span>

| <span data-ttu-id="14d64-113">属性</span><span class="sxs-lookup"><span data-stu-id="14d64-113">Property</span></span>  | <span data-ttu-id="14d64-114">类型</span><span class="sxs-lookup"><span data-stu-id="14d64-114">Type</span></span>   | <span data-ttu-id="14d64-115">说明</span><span class="sxs-lookup"><span data-stu-id="14d64-115">Description</span></span>                                                            |
|:----------|:-------|:-----------------------------------------------------------------------|
| <span data-ttu-id="14d64-116">name</span><span class="sxs-lookup"><span data-stu-id="14d64-116">name</span></span>      | <span data-ttu-id="14d64-117">string</span><span class="sxs-lookup"><span data-stu-id="14d64-117">string</span></span> | <span data-ttu-id="14d64-118">此项在 `/drive/special` 集合中的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="14d64-118">The unique identifier for this item in the `/drive/special` collection</span></span> |

## <a name="special-folders"></a><span data-ttu-id="14d64-119">特殊文件夹</span><span class="sxs-lookup"><span data-stu-id="14d64-119">Special folders</span></span>

<span data-ttu-id="14d64-120">以下是 OneDrive 个人版和 OneDrive for Business 中可用的特殊文件夹。</span><span class="sxs-lookup"><span data-stu-id="14d64-120">Here are the special folders available in OneDrive Personal and OneDrive for Business.</span></span>

| <span data-ttu-id="14d64-121">名称</span><span class="sxs-lookup"><span data-stu-id="14d64-121">Name</span></span>        | <span data-ttu-id="14d64-122">文件夹 ID</span><span class="sxs-lookup"><span data-stu-id="14d64-122">Folder id</span></span>    | <span data-ttu-id="14d64-123">说明</span><span class="sxs-lookup"><span data-stu-id="14d64-123">Description</span></span>                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| <span data-ttu-id="14d64-124">应用根目录</span><span class="sxs-lookup"><span data-stu-id="14d64-124">App Root</span></span>    | `approot`    | <span data-ttu-id="14d64-p104">应用程序的个人文件夹。通常位于 `/Apps/{Application Name}` 中</span><span class="sxs-lookup"><span data-stu-id="14d64-p104">The application's personal folder. Usually in `/Apps/{Application Name}`</span></span> |
| <span data-ttu-id="14d64-127">本机照片</span><span class="sxs-lookup"><span data-stu-id="14d64-127">Camera Roll</span></span> | `cameraroll` | <span data-ttu-id="14d64-p105">本机照片备份文件夹。不适用于 OneDrive for Business。</span><span class="sxs-lookup"><span data-stu-id="14d64-p105">The Camera Roll Backup folder. Not available in OneDrive for Business.</span></span>   |
| <span data-ttu-id="14d64-130">文档</span><span class="sxs-lookup"><span data-stu-id="14d64-130">Documents</span></span>   | `documents`  | <span data-ttu-id="14d64-131">文档文件夹。</span><span class="sxs-lookup"><span data-stu-id="14d64-131">The Documents folder.</span></span>                                                    |
| <span data-ttu-id="14d64-132">音乐</span><span class="sxs-lookup"><span data-stu-id="14d64-132">Music</span></span>       | `music`      | <span data-ttu-id="14d64-p106">音乐文件夹。不适用于 OneDrive for Business。</span><span class="sxs-lookup"><span data-stu-id="14d64-p106">The Music folder. Not available in OneDrive for Business.</span></span>                |
| <span data-ttu-id="14d64-135">照片</span><span class="sxs-lookup"><span data-stu-id="14d64-135">Photos</span></span>      | `photos`     | <span data-ttu-id="14d64-136">照片文件夹。</span><span class="sxs-lookup"><span data-stu-id="14d64-136">The Photos folder.</span></span>                                                       |

## <a name="remarks"></a><span data-ttu-id="14d64-137">注解</span><span class="sxs-lookup"><span data-stu-id="14d64-137">Remarks</span></span> 

<span data-ttu-id="14d64-138">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="14d64-138">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


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
