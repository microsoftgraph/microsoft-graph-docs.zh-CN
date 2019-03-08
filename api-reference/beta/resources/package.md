---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 程序包
localization_priority: Normal
ms.openlocfilehash: bcfc1a1e754286566c8b24b9b00c7f2eb0721316
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482383"
---
# <a name="package-resource-type"></a><span data-ttu-id="b542b-102">包资源类型</span><span class="sxs-lookup"><span data-stu-id="b542b-102">Package resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b542b-103">**包** 资源指示 DriveItem 是项的“包”或集合中的顶级项，应视为集合而不是单独的项。</span><span class="sxs-lookup"><span data-stu-id="b542b-103">The **Package** resource indicates that a DriveItem is the top level item in a "package" or a collection of items that should be treated as a collection instead of individual items.</span></span>

<span data-ttu-id="b542b-p101">包的一个示例是 OneNote 笔记本。笔记本由表示笔记本内容的文件和文件夹组成，表示该笔记本的顶级项具有**包** facet，以向客户端指示这是应被特殊处理的数据集。</span><span class="sxs-lookup"><span data-stu-id="b542b-p101">An example of a package is a OneNote notebook. While the notebook is made up of files and folders that represent the contents of the notebook, the top level item that represents the notebook has a **package** facet to indicate to clients that this is a collection of data that should be treated special.</span></span>

<span data-ttu-id="b542b-106">具有**包** facet 的 DriveItems 不包括**文件夹**或**文件** facet，但在概念上与具有**文件夹** facet 的项类似。</span><span class="sxs-lookup"><span data-stu-id="b542b-106">DriveItems with the **package** facet do not include a **folder** or **file** facet but are conceptually similar to an item with a **folder** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b542b-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b542b-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

| <span data-ttu-id="b542b-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="b542b-108">Property Name</span></span> | <span data-ttu-id="b542b-109">类型</span><span class="sxs-lookup"><span data-stu-id="b542b-109">Type</span></span>   | <span data-ttu-id="b542b-110">说明</span><span class="sxs-lookup"><span data-stu-id="b542b-110">Description</span></span>                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b542b-111">**类型**</span><span class="sxs-lookup"><span data-stu-id="b542b-111">**type**</span></span>      | <span data-ttu-id="b542b-112">string</span><span class="sxs-lookup"><span data-stu-id="b542b-112">string</span></span> | <span data-ttu-id="b542b-p102">表示包类型的字符串。虽然 `oneNote` 是当前唯一定义的值，但应该预见会返回其他包类型并进行相应处理。</span><span class="sxs-lookup"><span data-stu-id="b542b-p102">An string indicating the type of package. While `oneNote` is the only currently defined value, you should expect other package types to be returned and handle them accordingly.</span></span> |

## <a name="remarks"></a><span data-ttu-id="b542b-115">注解</span><span class="sxs-lookup"><span data-stu-id="b542b-115">Remarks</span></span> 

<span data-ttu-id="b542b-116">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="b542b-116">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/beta/resources/package.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
