---
author: JeremyKelley
ms.date: 09/10/2017
title: 程序包
localization_priority: Normal
description: " 或应视为集合而不是单个项目的项目集合。"
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e248c74add209690dbd7c3cc11d8056c5ca30dcc
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239812"
---
# <a name="package-resource-type"></a><span data-ttu-id="ca1d6-103">包资源类型</span><span class="sxs-lookup"><span data-stu-id="ca1d6-103">Package resource type</span></span>

<span data-ttu-id="ca1d6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca1d6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ca1d6-105">**包** 资源指示 DriveItem 是项的“包”或集合中的顶级项，应视为集合而不是单独的项。</span><span class="sxs-lookup"><span data-stu-id="ca1d6-105">The **Package** resource indicates that a DriveItem is the top level item in a "package" or a collection of items that should be treated as a collection instead of individual items.</span></span>

<span data-ttu-id="ca1d6-p101">包的一个示例是 OneNote 笔记本。笔记本由表示笔记本内容的文件和文件夹组成，表示该笔记本的顶级项具有 **包** facet，以向客户端指示这是应被特殊处理的数据集。</span><span class="sxs-lookup"><span data-stu-id="ca1d6-p101">An example of a package is a OneNote notebook. While the notebook is made up of files and folders that represent the contents of the notebook, the top level item that represents the notebook has a **package** facet to indicate to clients that this is a collection of data that should be treated special.</span></span>

<span data-ttu-id="ca1d6-108">具有 **包** facet 的 DriveItems 不包括 **文件夹** 或 **文件** facet，但在概念上与具有 **文件夹** facet 的项类似。</span><span class="sxs-lookup"><span data-stu-id="ca1d6-108">DriveItems with the **package** facet do not include a **folder** or **file** facet but are conceptually similar to an item with a **folder** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca1d6-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ca1d6-109">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

## <a name="properties"></a><span data-ttu-id="ca1d6-110">属性</span><span class="sxs-lookup"><span data-stu-id="ca1d6-110">Properties</span></span>

| <span data-ttu-id="ca1d6-111">属性名</span><span class="sxs-lookup"><span data-stu-id="ca1d6-111">Property Name</span></span> | <span data-ttu-id="ca1d6-112">类型</span><span class="sxs-lookup"><span data-stu-id="ca1d6-112">Type</span></span>   | <span data-ttu-id="ca1d6-113">说明</span><span class="sxs-lookup"><span data-stu-id="ca1d6-113">Description</span></span>                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ca1d6-114">类型</span><span class="sxs-lookup"><span data-stu-id="ca1d6-114">type</span></span>          | <span data-ttu-id="ca1d6-115">string</span><span class="sxs-lookup"><span data-stu-id="ca1d6-115">string</span></span> | <span data-ttu-id="ca1d6-116">一个指示程序包类型的字符串。</span><span class="sxs-lookup"><span data-stu-id="ca1d6-116">A string indicating the type of package.</span></span> <span data-ttu-id="ca1d6-117">虽然 `oneNote` 是当前唯一定义的值，但应该预见会返回其他包类型并进行相应处理。</span><span class="sxs-lookup"><span data-stu-id="ca1d6-117">While `oneNote` is the only currently defined value, you should expect other package types to be returned and handle them accordingly.</span></span> |

## <a name="remarks"></a><span data-ttu-id="ca1d6-118">注解</span><span class="sxs-lookup"><span data-stu-id="ca1d6-118">Remarks</span></span> 

<span data-ttu-id="ca1d6-119">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="ca1d6-119">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "tocPath": "Facets/Package"
} -->

