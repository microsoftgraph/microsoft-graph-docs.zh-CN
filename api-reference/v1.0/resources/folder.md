---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Folder
ms.openlocfilehash: dc90624b14a88d06b45302f421a7e3fcfa802a67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007680"
---
# <a name="folder-resource-type"></a><span data-ttu-id="701d9-102">Folder 资源类型</span><span class="sxs-lookup"><span data-stu-id="701d9-102">Folder resource type</span></span>

<span data-ttu-id="701d9-p101">**文件夹**资源将与文件夹相关的数据项分组到一个单一结构。具有非 null **文件夹**方面的 [**DriveItems**](driveitem.md) 是其他 DriveItems 的容器。</span><span class="sxs-lookup"><span data-stu-id="701d9-p101">The **Folder** resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="701d9-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="701d9-105">JSON representation</span></span>

<span data-ttu-id="701d9-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="701d9-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="701d9-107">属性</span><span class="sxs-lookup"><span data-stu-id="701d9-107">Properties</span></span>

| <span data-ttu-id="701d9-108">属性</span><span class="sxs-lookup"><span data-stu-id="701d9-108">Property</span></span>       | <span data-ttu-id="701d9-109">类型</span><span class="sxs-lookup"><span data-stu-id="701d9-109">Type</span></span>           | <span data-ttu-id="701d9-110">说明</span><span class="sxs-lookup"><span data-stu-id="701d9-110">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="701d9-111">**childCount**</span><span class="sxs-lookup"><span data-stu-id="701d9-111">**childCount**</span></span> | <span data-ttu-id="701d9-112">Int32</span><span class="sxs-lookup"><span data-stu-id="701d9-112">Int32</span></span>          | <span data-ttu-id="701d9-113">此容器包含的直接子项数量。</span><span class="sxs-lookup"><span data-stu-id="701d9-113">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="701d9-114">**view**</span><span class="sxs-lookup"><span data-stu-id="701d9-114">**view**</span></span>       | <span data-ttu-id="701d9-115">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="701d9-115">[folderView][]</span></span> | <span data-ttu-id="701d9-116">用于定义文件夹的推荐视图的属性集合。</span><span class="sxs-lookup"><span data-stu-id="701d9-116">A collection of properties defining the recommended view for the folder.</span></span>

## <a name="remarks"></a><span data-ttu-id="701d9-117">备注</span><span class="sxs-lookup"><span data-stu-id="701d9-117">Remarks</span></span> 

<span data-ttu-id="701d9-118">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem][]。</span><span class="sxs-lookup"><span data-stu-id="701d9-118">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The Folder facet describes properties of a folder",
  "keywords": "folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Folder"
} -->
