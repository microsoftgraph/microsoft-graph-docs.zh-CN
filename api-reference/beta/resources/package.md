---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 程序包
localization_priority: Normal
ms.openlocfilehash: 67e82faa3f51eeae71c2dcb22ecb7a973e2070bb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516600"
---
# <a name="package-resource-type"></a><span data-ttu-id="632ce-102">包资源类型</span><span class="sxs-lookup"><span data-stu-id="632ce-102">Package resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="632ce-103">**包** 资源指示 DriveItem 是项的“包”或集合中的顶级项，应视为集合而不是单独的项。</span><span class="sxs-lookup"><span data-stu-id="632ce-103">The **Package** resource indicates that a DriveItem is the top level item in a "package" or a collection of items that should be treated as a collection instead of individual items.</span></span>

<span data-ttu-id="632ce-p101">例如，包可以是 OneNote 笔记本。笔记本由表示笔记本内容的文件和文件夹组成，而表示笔记本的顶级项则具有 **Package** Facet，以向客户端指明这是应特殊处理的数据集合。</span><span class="sxs-lookup"><span data-stu-id="632ce-p101">An example of a package is a OneNote notebook. While the notebook is made up of files and folders that represent the contents of the notebook, the top level item that represents the notebook has a **package** facet to indicate to clients that this is a collection of data that should be treated special.</span></span>

<span data-ttu-id="632ce-106">具有**包** facet 的 DriveItems 不包括**文件夹**或**文件** facet，但在概念上与具有**文件夹** facet 的项类似。</span><span class="sxs-lookup"><span data-stu-id="632ce-106">DriveItems with the **package** facet do not include a **folder** or **file** facet but are conceptually similar to an item with a **folder** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="632ce-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="632ce-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

| <span data-ttu-id="632ce-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="632ce-108">Property Name</span></span> | <span data-ttu-id="632ce-109">类型</span><span class="sxs-lookup"><span data-stu-id="632ce-109">Type</span></span>   | <span data-ttu-id="632ce-110">说明</span><span class="sxs-lookup"><span data-stu-id="632ce-110">Description</span></span>                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="632ce-111">**类型**</span><span class="sxs-lookup"><span data-stu-id="632ce-111">**type**</span></span>      | <span data-ttu-id="632ce-112">string</span><span class="sxs-lookup"><span data-stu-id="632ce-112">string</span></span> | <span data-ttu-id="632ce-p102">表示包类型的字符串。虽然 `oneNote` 是当前唯一定义的值，但应该预见会返回其他包类型并进行相应处理。</span><span class="sxs-lookup"><span data-stu-id="632ce-p102">An string indicating the type of package. While `oneNote` is the only currently defined value, you should expect other package types to be returned and handle them accordingly.</span></span> |

## <a name="remarks"></a><span data-ttu-id="632ce-115">注解</span><span class="sxs-lookup"><span data-stu-id="632ce-115">Remarks</span></span> 

<span data-ttu-id="632ce-116">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="632ce-116">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


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
