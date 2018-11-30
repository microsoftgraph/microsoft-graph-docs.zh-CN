---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 程序包
ms.openlocfilehash: fe26cf0dc5de00673d5c3c2ae4a90ac80a62897f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047812"
---
# <a name="package-resource-type"></a><span data-ttu-id="d4764-102">包资源类型</span><span class="sxs-lookup"><span data-stu-id="d4764-102">Package resource type</span></span>

> <span data-ttu-id="d4764-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d4764-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4764-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d4764-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d4764-105">**包** 资源指示 DriveItem 是项的“包”或集合中的顶级项，应视为集合而不是单独的项。</span><span class="sxs-lookup"><span data-stu-id="d4764-105">The **Package** resource indicates that a DriveItem is the top level item in a "package" or a collection of items that should be treated as a collection instead of individual items.</span></span>

<span data-ttu-id="d4764-106">包的一个示例是 OneNote 笔记本。</span><span class="sxs-lookup"><span data-stu-id="d4764-106">An example of a package is a OneNote notebook.</span></span> <span data-ttu-id="d4764-107">笔记本由表示笔记本内容的文件和文件夹组成，表示该笔记本的顶级项具有**包** facet，以向客户端指示这是应被特殊处理的数据集。</span><span class="sxs-lookup"><span data-stu-id="d4764-107">While the notebook is made up of files and folders that represent the contents of the notebook, the top level item that represents the notebook has a **package** facet to indicate to clients that this is a collection of data that should be treated special.</span></span>

<span data-ttu-id="d4764-108">具有**包** facet 的 DriveItems 不包括**文件夹**或**文件** facet，但在概念上与具有**文件夹** facet 的项类似。</span><span class="sxs-lookup"><span data-stu-id="d4764-108">DriveItems with the **package** facet do not include a **folder** or **file** facet but are conceptually similar to an item with a **folder** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4764-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4764-109">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

| <span data-ttu-id="d4764-110">属性名称</span><span class="sxs-lookup"><span data-stu-id="d4764-110">Property Name</span></span> | <span data-ttu-id="d4764-111">类型</span><span class="sxs-lookup"><span data-stu-id="d4764-111">Type</span></span>   | <span data-ttu-id="d4764-112">说明</span><span class="sxs-lookup"><span data-stu-id="d4764-112">Description</span></span>                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d4764-113">**类型**</span><span class="sxs-lookup"><span data-stu-id="d4764-113">**type**</span></span>      | <span data-ttu-id="d4764-114">string</span><span class="sxs-lookup"><span data-stu-id="d4764-114">string</span></span> | <span data-ttu-id="d4764-p103">表示包类型的字符串。虽然 `oneNote` 是当前唯一定义的值，但应该预见会返回其他包类型并进行相应处理。</span><span class="sxs-lookup"><span data-stu-id="d4764-p103">An string indicating the type of package. While `oneNote` is the only currently defined value, you should expect other package types to be returned and handle them accordingly.</span></span> |

## <a name="remarks"></a><span data-ttu-id="d4764-117">注解</span><span class="sxs-lookup"><span data-stu-id="d4764-117">Remarks</span></span> 

<span data-ttu-id="d4764-118">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="d4764-118">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation"
} -->
