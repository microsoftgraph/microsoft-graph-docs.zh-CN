---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Package
localization_priority: Normal
description: " 或应被视为集合而不是单个项目的项的集合。"
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d8eff13e0cfdc6b355cc289833e7b3050ded2641
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035663"
---
# <a name="package-resource-type"></a><span data-ttu-id="66060-103">包资源类型</span><span class="sxs-lookup"><span data-stu-id="66060-103">Package resource type</span></span>

<span data-ttu-id="66060-104">**包** 资源指示 DriveItem 是项的“包”或集合中的顶级项，应视为集合而不是单独的项。</span><span class="sxs-lookup"><span data-stu-id="66060-104">The **Package** resource indicates that a DriveItem is the top level item in a "package" or a collection of items that should be treated as a collection instead of individual items.</span></span>

<span data-ttu-id="66060-p101">包的一个示例是 OneNote 笔记本。笔记本由表示笔记本内容的文件和文件夹组成，表示该笔记本的顶级项具有**包** facet，以向客户端指示这是应被特殊处理的数据集。</span><span class="sxs-lookup"><span data-stu-id="66060-p101">An example of a package is a OneNote notebook. While the notebook is made up of files and folders that represent the contents of the notebook, the top level item that represents the notebook has a **package** facet to indicate to clients that this is a collection of data that should be treated special.</span></span>

<span data-ttu-id="66060-107">具有**包** facet 的 DriveItems 不包括**文件夹**或**文件** facet，但在概念上与具有**文件夹** facet 的项类似。</span><span class="sxs-lookup"><span data-stu-id="66060-107">DriveItems with the **package** facet do not include a **folder** or **file** facet but are conceptually similar to an item with a **folder** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="66060-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="66060-108">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

## <a name="properties"></a><span data-ttu-id="66060-109">属性</span><span class="sxs-lookup"><span data-stu-id="66060-109">Properties</span></span>

| <span data-ttu-id="66060-110">属性名称</span><span class="sxs-lookup"><span data-stu-id="66060-110">Property Name</span></span> | <span data-ttu-id="66060-111">类型</span><span class="sxs-lookup"><span data-stu-id="66060-111">Type</span></span>   | <span data-ttu-id="66060-112">说明</span><span class="sxs-lookup"><span data-stu-id="66060-112">Description</span></span>                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="66060-113">类型</span><span class="sxs-lookup"><span data-stu-id="66060-113">type</span></span>          | <span data-ttu-id="66060-114">string</span><span class="sxs-lookup"><span data-stu-id="66060-114">string</span></span> | <span data-ttu-id="66060-115">一个指示包的类型的字符串。</span><span class="sxs-lookup"><span data-stu-id="66060-115">A string indicating the type of package.</span></span> <span data-ttu-id="66060-116">虽然 `oneNote` 是当前唯一定义的值，但应该预见会返回其他包类型并进行相应处理。</span><span class="sxs-lookup"><span data-stu-id="66060-116">While `oneNote` is the only currently defined value, you should expect other package types to be returned and handle them accordingly.</span></span> |

## <a name="remarks"></a><span data-ttu-id="66060-117">注解</span><span class="sxs-lookup"><span data-stu-id="66060-117">Remarks</span></span> 

<span data-ttu-id="66060-118">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="66060-118">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "tocPath": "Facets/Package"
} -->
