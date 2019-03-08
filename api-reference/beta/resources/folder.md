---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Folder
localization_priority: Normal
ms.openlocfilehash: b78e6038a8f8f9a91883dd29faeebe3d5db3ca04
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481214"
---
# <a name="folder-resource-type"></a><span data-ttu-id="40db7-102">文件夹资源类型</span><span class="sxs-lookup"><span data-stu-id="40db7-102">Folder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40db7-p101">**文件夹**资源将与文件夹相关的数据项分组到一个单一结构。具有非 null **文件夹**方面的 **[DriveItems](driveitem.md)** 是其他 DriveItems 的容器。</span><span class="sxs-lookup"><span data-stu-id="40db7-p101">The **Folder** resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="40db7-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="40db7-105">JSON representation</span></span>

<span data-ttu-id="40db7-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="40db7-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.folder"
}-->

```json
{
  "childCount": 1024,
  "view": { "@odata.type": "microsoft.graph.folderView" }
}
```

## <a name="properties"></a><span data-ttu-id="40db7-107">属性</span><span class="sxs-lookup"><span data-stu-id="40db7-107">Properties</span></span>

| <span data-ttu-id="40db7-108">属性</span><span class="sxs-lookup"><span data-stu-id="40db7-108">Property</span></span>       | <span data-ttu-id="40db7-109">类型</span><span class="sxs-lookup"><span data-stu-id="40db7-109">Type</span></span>           | <span data-ttu-id="40db7-110">说明</span><span class="sxs-lookup"><span data-stu-id="40db7-110">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="40db7-111">**childCount**</span><span class="sxs-lookup"><span data-stu-id="40db7-111">**childCount**</span></span> | <span data-ttu-id="40db7-112">Int64</span><span class="sxs-lookup"><span data-stu-id="40db7-112">Int64</span></span>          | <span data-ttu-id="40db7-113">此容器包含的直接子项数量。</span><span class="sxs-lookup"><span data-stu-id="40db7-113">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="40db7-114">**view**</span><span class="sxs-lookup"><span data-stu-id="40db7-114">**view**</span></span>       | <span data-ttu-id="40db7-115">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="40db7-115">[folderView][]</span></span> | <span data-ttu-id="40db7-116">用于定义文件夹的推荐视图的属性集合。</span><span class="sxs-lookup"><span data-stu-id="40db7-116">A collection of properties defining the recommended view for the folder.</span></span>


## <a name="remarks"></a><span data-ttu-id="40db7-117">注解</span><span class="sxs-lookup"><span data-stu-id="40db7-117">Remarks</span></span> 

<span data-ttu-id="40db7-118">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem][]。</span><span class="sxs-lookup"><span data-stu-id="40db7-118">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "folder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/folder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
