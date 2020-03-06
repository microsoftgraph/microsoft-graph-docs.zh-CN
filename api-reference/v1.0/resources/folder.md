---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Folder
localization_priority: Normal
description: '文件夹资源将与文件夹相关的数据项分组到一个单一结构。 '
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1ee34252671477a1efb83daf056330b499d94966
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531401"
---
# <a name="folder-resource-type"></a><span data-ttu-id="274b9-103">文件夹资源类型</span><span class="sxs-lookup"><span data-stu-id="274b9-103">Folder resource type</span></span>

<span data-ttu-id="274b9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="274b9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="274b9-p101">**文件夹**资源将与文件夹相关的数据项分组到一个单一结构。具有非 null **文件夹**方面的 **[DriveItems](driveitem.md)** 是其他 DriveItems 的容器。</span><span class="sxs-lookup"><span data-stu-id="274b9-p101">The **Folder** resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="274b9-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="274b9-107">JSON representation</span></span>

<span data-ttu-id="274b9-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="274b9-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="274b9-109">属性</span><span class="sxs-lookup"><span data-stu-id="274b9-109">Properties</span></span>

| <span data-ttu-id="274b9-110">属性</span><span class="sxs-lookup"><span data-stu-id="274b9-110">Property</span></span>       | <span data-ttu-id="274b9-111">类型</span><span class="sxs-lookup"><span data-stu-id="274b9-111">Type</span></span>           | <span data-ttu-id="274b9-112">说明</span><span class="sxs-lookup"><span data-stu-id="274b9-112">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="274b9-113">**childCount**</span><span class="sxs-lookup"><span data-stu-id="274b9-113">**childCount**</span></span> | <span data-ttu-id="274b9-114">Int32</span><span class="sxs-lookup"><span data-stu-id="274b9-114">Int32</span></span>          | <span data-ttu-id="274b9-115">此容器包含的直接子项数量。</span><span class="sxs-lookup"><span data-stu-id="274b9-115">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="274b9-116">**view**</span><span class="sxs-lookup"><span data-stu-id="274b9-116">**view**</span></span>       | <span data-ttu-id="274b9-117">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="274b9-117">[folderView][]</span></span> | <span data-ttu-id="274b9-118">用于定义文件夹的推荐视图的属性集合。</span><span class="sxs-lookup"><span data-stu-id="274b9-118">A collection of properties defining the recommended view for the folder.</span></span>

## <a name="remarks"></a><span data-ttu-id="274b9-119">注解</span><span class="sxs-lookup"><span data-stu-id="274b9-119">Remarks</span></span> 

<span data-ttu-id="274b9-120">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem][]。</span><span class="sxs-lookup"><span data-stu-id="274b9-120">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The Folder facet describes properties of a folder",
  "keywords": "folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Folder"
} -->
