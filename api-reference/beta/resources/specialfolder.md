---
author: JeremyKelley
description: 将特殊文件夹相关的数据项分组到单个结构中。
title: specialFolder 资源类型
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: d9552c79588f8533980879c2ed49ed32fdfe7927
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236269"
---
# <a name="specialfolder-resource-type"></a><span data-ttu-id="045aa-103">specialFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="045aa-103">specialFolder resource type</span></span>

<span data-ttu-id="045aa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="045aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="045aa-105">将特殊文件夹相关的数据项分组到单个结构中。</span><span class="sxs-lookup"><span data-stu-id="045aa-105">Groups special folder-related data items into a single structure.</span></span>

<span data-ttu-id="045aa-106">如果 **driveItem** 具有非 null **specialFolder** Facet，则该项表示名为 (文件夹) 对象。</span><span class="sxs-lookup"><span data-stu-id="045aa-106">If a **driveItem** has a non-null **specialFolder** facet, the item represents a special (named) folder.</span></span>
<span data-ttu-id="045aa-107">可直接通过 [special folders 集合](../api/drive-get-specialfolder.md) 访问特殊文件夹。</span><span class="sxs-lookup"><span data-stu-id="045aa-107">Special folders can be accessed directly via the [special folders collection](../api/drive-get-specialfolder.md).</span></span>

<span data-ttu-id="045aa-p102">特殊文件夹可提供简单别名，因此无需按路径查找（需要本地化）文件夹或通过 ID 引用文件夹来访问已知文件夹。如果特殊文件夹被重命名或移到驱动器中的其他位置，此语法将继续返回该文件夹。</span><span class="sxs-lookup"><span data-stu-id="045aa-p102">Special folders provide simple aliases to access well-known folders without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to return that folder.</span></span>

<span data-ttu-id="045aa-p103">应用程序第一次尝试向特殊文件夹中写入内容时，如果特殊文件夹不存在，系统会自动创建特殊文件夹。如果用户删除某个特殊文件夹，再次向其写入内容时会重新创建特殊文件夹。</span><span class="sxs-lookup"><span data-stu-id="045aa-p103">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

[!INCLUDE [files-special-folder-list](../includes/files-special-folder-list.md)]

><span data-ttu-id="045aa-112">**注意：** 如果应用仅请求 **Files.Read** 范围，而请求特殊文件夹不存在，则响应将是 `403 Forbidden` 错误。</span><span class="sxs-lookup"><span data-stu-id="045aa-112">**Note:** If your app has only requested **Files.Read** scope and requests a special folder that doesn't exist, the response will be a `403 Forbidden` error.</span></span>

## <a name="properties"></a><span data-ttu-id="045aa-113">属性</span><span class="sxs-lookup"><span data-stu-id="045aa-113">Properties</span></span>

| <span data-ttu-id="045aa-114">属性</span><span class="sxs-lookup"><span data-stu-id="045aa-114">Property</span></span>  | <span data-ttu-id="045aa-115">类型</span><span class="sxs-lookup"><span data-stu-id="045aa-115">Type</span></span>   | <span data-ttu-id="045aa-116">说明</span><span class="sxs-lookup"><span data-stu-id="045aa-116">Description</span></span>                                                            |
|:----------|:-------|:-----------------------------------------------------------------------|
| <span data-ttu-id="045aa-117">name</span><span class="sxs-lookup"><span data-stu-id="045aa-117">name</span></span>      | <span data-ttu-id="045aa-118">string</span><span class="sxs-lookup"><span data-stu-id="045aa-118">string</span></span> | <span data-ttu-id="045aa-119">此项在 `/drive/special` 集合中的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="045aa-119">The unique identifier for this item in the `/drive/special` collection</span></span> |


## <a name="json-representation"></a><span data-ttu-id="045aa-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="045aa-120">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="045aa-121">另请参阅</span><span class="sxs-lookup"><span data-stu-id="045aa-121">See also</span></span> 

<span data-ttu-id="045aa-122">有关 driveItem 上 Facet 的信息，请参阅 [driveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="045aa-122">For more information about the facets on a driveItem, see [driveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The SpecialFolder facet provides information about folders accessible as special folders.",
  "keywords": "special folder,item,facet",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


