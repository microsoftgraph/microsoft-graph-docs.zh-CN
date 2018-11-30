---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Folder
ms.openlocfilehash: 834b2cd7c81a947ca1e6d4619f39a8533677e6c3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047537"
---
# <a name="folder-resource-type"></a><span data-ttu-id="b86d8-102">Folder 资源类型</span><span class="sxs-lookup"><span data-stu-id="b86d8-102">Folder resource type</span></span>

> <span data-ttu-id="b86d8-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b86d8-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b86d8-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b86d8-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b86d8-p102">**文件夹**资源将与文件夹相关的数据项分组到一个单一结构。具有非 null **文件夹**方面的 [**DriveItems**](driveitem.md) 是其他 DriveItems 的容器。</span><span class="sxs-lookup"><span data-stu-id="b86d8-p102">The **Folder** resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b86d8-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b86d8-107">JSON representation</span></span>

<span data-ttu-id="b86d8-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b86d8-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="b86d8-109">属性</span><span class="sxs-lookup"><span data-stu-id="b86d8-109">Properties</span></span>

| <span data-ttu-id="b86d8-110">属性</span><span class="sxs-lookup"><span data-stu-id="b86d8-110">Property</span></span>       | <span data-ttu-id="b86d8-111">类型</span><span class="sxs-lookup"><span data-stu-id="b86d8-111">Type</span></span>           | <span data-ttu-id="b86d8-112">说明</span><span class="sxs-lookup"><span data-stu-id="b86d8-112">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="b86d8-113">**childCount**</span><span class="sxs-lookup"><span data-stu-id="b86d8-113">**childCount**</span></span> | <span data-ttu-id="b86d8-114">Int64</span><span class="sxs-lookup"><span data-stu-id="b86d8-114">Int64</span></span>          | <span data-ttu-id="b86d8-115">此容器包含的直接子项数量。</span><span class="sxs-lookup"><span data-stu-id="b86d8-115">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="b86d8-116">**view**</span><span class="sxs-lookup"><span data-stu-id="b86d8-116">**view**</span></span>       | <span data-ttu-id="b86d8-117">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="b86d8-117">[folderView][]</span></span> | <span data-ttu-id="b86d8-118">用于定义文件夹的推荐视图的属性集合。</span><span class="sxs-lookup"><span data-stu-id="b86d8-118">A collection of properties defining the recommended view for the folder.</span></span>


## <a name="remarks"></a><span data-ttu-id="b86d8-119">备注</span><span class="sxs-lookup"><span data-stu-id="b86d8-119">Remarks</span></span> 

<span data-ttu-id="b86d8-120">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem][]。</span><span class="sxs-lookup"><span data-stu-id="b86d8-120">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "folder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
