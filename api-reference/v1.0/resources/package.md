---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 程序包
ms.openlocfilehash: 12ae750a0f4fbe0e951554308d4041928c31a16d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010540"
---
# <a name="package-resource-type"></a><span data-ttu-id="4b3b8-102">包资源类型</span><span class="sxs-lookup"><span data-stu-id="4b3b8-102">Package resource type</span></span>

<span data-ttu-id="4b3b8-103">**包** 资源指示 DriveItem 是项的“包”或集合中的顶级项，应视为集合而不是单独的项。</span><span class="sxs-lookup"><span data-stu-id="4b3b8-103">The **Package** resource indicates that a DriveItem is the top level item in a "package" or a collection of items that should be treated as a collection instead of individual items.</span></span>

<span data-ttu-id="4b3b8-104">包的一个示例是 OneNote 笔记本。</span><span class="sxs-lookup"><span data-stu-id="4b3b8-104">An example of a package is a OneNote notebook.</span></span> <span data-ttu-id="4b3b8-105">笔记本由表示笔记本内容的文件和文件夹组成，表示该笔记本的顶级项具有**包** facet，以向客户端指示这是应被特殊处理的数据集。</span><span class="sxs-lookup"><span data-stu-id="4b3b8-105">While the notebook is made up of files and folders that represent the contents of the notebook, the top level item that represents the notebook has a **package** facet to indicate to clients that this is a collection of data that should be treated special.</span></span>

<span data-ttu-id="4b3b8-106">具有**包** facet 的 DriveItems 不包括**文件夹**或**文件** facet，但在概念上与具有**文件夹** facet 的项类似。</span><span class="sxs-lookup"><span data-stu-id="4b3b8-106">DriveItems with the **package** facet do not include a **folder** or **file** facet but are conceptually similar to an item with a **folder** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b3b8-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4b3b8-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

## <a name="properties"></a><span data-ttu-id="4b3b8-108">属性</span><span class="sxs-lookup"><span data-stu-id="4b3b8-108">Properties</span></span>

| <span data-ttu-id="4b3b8-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="4b3b8-109">Property Name</span></span> | <span data-ttu-id="4b3b8-110">类型</span><span class="sxs-lookup"><span data-stu-id="4b3b8-110">Type</span></span>   | <span data-ttu-id="4b3b8-111">说明</span><span class="sxs-lookup"><span data-stu-id="4b3b8-111">Description</span></span>                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4b3b8-112">type</span><span class="sxs-lookup"><span data-stu-id="4b3b8-112">type</span></span>          | <span data-ttu-id="4b3b8-113">string</span><span class="sxs-lookup"><span data-stu-id="4b3b8-113">string</span></span> | <span data-ttu-id="4b3b8-114">指示包的类型的字符串。</span><span class="sxs-lookup"><span data-stu-id="4b3b8-114">A string indicating the type of package.</span></span> <span data-ttu-id="4b3b8-115">时`oneNote`是仅当前定义的值，则应产生预期其他包类型返回并据此处理它们。</span><span class="sxs-lookup"><span data-stu-id="4b3b8-115">While `oneNote` is the only currently defined value, you should expect other package types to be returned and handle them accordingly.</span></span> |

## <a name="remarks"></a><span data-ttu-id="4b3b8-116">备注</span><span class="sxs-lookup"><span data-stu-id="4b3b8-116">Remarks</span></span> 

<span data-ttu-id="4b3b8-117">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="4b3b8-117">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "tocPath": "Facets/Package"
} -->
