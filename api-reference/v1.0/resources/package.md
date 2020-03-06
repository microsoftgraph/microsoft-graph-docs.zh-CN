---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 程序包
localization_priority: Normal
description: " 或应被视为集合而不是单个项目的项的集合。"
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 10e99df4a2411fd63e8b8a2ad78d2aa5f0684571
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534102"
---
# <a name="package-resource-type"></a><span data-ttu-id="6c9dc-103">包资源类型</span><span class="sxs-lookup"><span data-stu-id="6c9dc-103">Package resource type</span></span>

<span data-ttu-id="6c9dc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c9dc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6c9dc-105">**包** 资源指示 DriveItem 是项的“包”或集合中的顶级项，应视为集合而不是单独的项。</span><span class="sxs-lookup"><span data-stu-id="6c9dc-105">The **Package** resource indicates that a DriveItem is the top level item in a "package" or a collection of items that should be treated as a collection instead of individual items.</span></span>

<span data-ttu-id="6c9dc-p101">包的一个示例是 OneNote 笔记本。笔记本由表示笔记本内容的文件和文件夹组成，表示该笔记本的顶级项具有**包** facet，以向客户端指示这是应被特殊处理的数据集。</span><span class="sxs-lookup"><span data-stu-id="6c9dc-p101">An example of a package is a OneNote notebook. While the notebook is made up of files and folders that represent the contents of the notebook, the top level item that represents the notebook has a **package** facet to indicate to clients that this is a collection of data that should be treated special.</span></span>

<span data-ttu-id="6c9dc-108">具有**包** facet 的 DriveItems 不包括**文件夹**或**文件** facet，但在概念上与具有**文件夹** facet 的项类似。</span><span class="sxs-lookup"><span data-stu-id="6c9dc-108">DriveItems with the **package** facet do not include a **folder** or **file** facet but are conceptually similar to an item with a **folder** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c9dc-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c9dc-109">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

## <a name="properties"></a><span data-ttu-id="6c9dc-110">属性</span><span class="sxs-lookup"><span data-stu-id="6c9dc-110">Properties</span></span>

| <span data-ttu-id="6c9dc-111">属性名</span><span class="sxs-lookup"><span data-stu-id="6c9dc-111">Property Name</span></span> | <span data-ttu-id="6c9dc-112">类型</span><span class="sxs-lookup"><span data-stu-id="6c9dc-112">Type</span></span>   | <span data-ttu-id="6c9dc-113">说明</span><span class="sxs-lookup"><span data-stu-id="6c9dc-113">Description</span></span>                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="6c9dc-114">类型</span><span class="sxs-lookup"><span data-stu-id="6c9dc-114">type</span></span>          | <span data-ttu-id="6c9dc-115">string</span><span class="sxs-lookup"><span data-stu-id="6c9dc-115">string</span></span> | <span data-ttu-id="6c9dc-116">一个指示包的类型的字符串。</span><span class="sxs-lookup"><span data-stu-id="6c9dc-116">A string indicating the type of package.</span></span> <span data-ttu-id="6c9dc-117">虽然 `oneNote` 是当前唯一定义的值，但应该预见会返回其他包类型并进行相应处理。</span><span class="sxs-lookup"><span data-stu-id="6c9dc-117">While `oneNote` is the only currently defined value, you should expect other package types to be returned and handle them accordingly.</span></span> |

## <a name="remarks"></a><span data-ttu-id="6c9dc-118">注解</span><span class="sxs-lookup"><span data-stu-id="6c9dc-118">Remarks</span></span> 

<span data-ttu-id="6c9dc-119">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="6c9dc-119">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "tocPath": "Facets/Package"
} -->
