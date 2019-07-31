---
author: JeremyKelley
description: '文件夹资源将与文件夹相关的数据项分组到一个单一结构。 '
ms.date: 09/10/2017
title: Folder
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: f9cbbba6ae20c56800a5f6f492319f47b7d8017c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971989"
---
# <a name="folder-resource-type"></a><span data-ttu-id="5716b-103">文件夹资源类型</span><span class="sxs-lookup"><span data-stu-id="5716b-103">Folder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5716b-p101">**文件夹**资源将与文件夹相关的数据项分组到一个单一结构。具有非 null **文件夹**方面的 **[DriveItems](driveitem.md)** 是其他 DriveItems 的容器。</span><span class="sxs-lookup"><span data-stu-id="5716b-p101">The **Folder** resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5716b-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5716b-106">JSON representation</span></span>

<span data-ttu-id="5716b-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5716b-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="5716b-108">属性</span><span class="sxs-lookup"><span data-stu-id="5716b-108">Properties</span></span>

| <span data-ttu-id="5716b-109">属性</span><span class="sxs-lookup"><span data-stu-id="5716b-109">Property</span></span>       | <span data-ttu-id="5716b-110">类型</span><span class="sxs-lookup"><span data-stu-id="5716b-110">Type</span></span>           | <span data-ttu-id="5716b-111">说明</span><span class="sxs-lookup"><span data-stu-id="5716b-111">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="5716b-112">**childCount**</span><span class="sxs-lookup"><span data-stu-id="5716b-112">**childCount**</span></span> | <span data-ttu-id="5716b-113">Int64</span><span class="sxs-lookup"><span data-stu-id="5716b-113">Int64</span></span>          | <span data-ttu-id="5716b-114">此容器包含的直接子项数量。</span><span class="sxs-lookup"><span data-stu-id="5716b-114">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="5716b-115">**view**</span><span class="sxs-lookup"><span data-stu-id="5716b-115">**view**</span></span>       | <span data-ttu-id="5716b-116">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="5716b-116">[folderView][]</span></span> | <span data-ttu-id="5716b-117">用于定义文件夹的推荐视图的属性集合。</span><span class="sxs-lookup"><span data-stu-id="5716b-117">A collection of properties defining the recommended view for the folder.</span></span>


## <a name="remarks"></a><span data-ttu-id="5716b-118">注解</span><span class="sxs-lookup"><span data-stu-id="5716b-118">Remarks</span></span> 

<span data-ttu-id="5716b-119">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem][]。</span><span class="sxs-lookup"><span data-stu-id="5716b-119">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "folder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
