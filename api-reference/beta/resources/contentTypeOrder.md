---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
ms.openlocfilehash: 9b92a8234c493ae9b0f396db7010e7bf717d5959
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514367"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="0e756-102">ContentTypeOrder 资源类型</span><span class="sxs-lookup"><span data-stu-id="0e756-102">ContentTypeOrder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e756-103">**contentTypeOrder** 资源指定在选择 UI 中显示内容类型的顺序。</span><span class="sxs-lookup"><span data-stu-id="0e756-103">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e756-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0e756-104">JSON representation</span></span>

<span data-ttu-id="0e756-105">下面是 **contentTypeOrder** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e756-105">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="0e756-106">属性</span><span class="sxs-lookup"><span data-stu-id="0e756-106">Properties</span></span>

| <span data-ttu-id="0e756-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="0e756-107">Property name</span></span> | <span data-ttu-id="0e756-108">类型</span><span class="sxs-lookup"><span data-stu-id="0e756-108">Type</span></span>    | <span data-ttu-id="0e756-109">说明</span><span class="sxs-lookup"><span data-stu-id="0e756-109">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="0e756-110">**default**</span><span class="sxs-lookup"><span data-stu-id="0e756-110">**default**</span></span>   | <span data-ttu-id="0e756-111">boolean</span><span class="sxs-lookup"><span data-stu-id="0e756-111">boolean</span></span> | <span data-ttu-id="0e756-112">这是否为默认的内容类型</span><span class="sxs-lookup"><span data-stu-id="0e756-112">Whether this is the default Content Type</span></span>
| <span data-ttu-id="0e756-113">**position**</span><span class="sxs-lookup"><span data-stu-id="0e756-113">**position**</span></span>  | <span data-ttu-id="0e756-114">Int32</span><span class="sxs-lookup"><span data-stu-id="0e756-114">Int32</span></span>   | <span data-ttu-id="0e756-115">指定在选择 UI 中显示内容类型的位置。</span><span class="sxs-lookup"><span data-stu-id="0e756-115">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder",
  "suppressions": [
    "Error: /api-reference/beta/resources/contentTypeOrder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
