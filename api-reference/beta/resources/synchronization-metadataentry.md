---
title: metadataEntry 资源类型
description: 给定对象的元数据。
localization_priority: Normal
ms.openlocfilehash: a6b9170144917e4c7b66bb52c1efb17d93167ef0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581750"
---
# <a name="metadataentry-resource-type"></a><span data-ttu-id="1fcfc-103">metadataEntry 资源类型</span><span class="sxs-lookup"><span data-stu-id="1fcfc-103">metadataEntry resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fcfc-104">给定对象的元数据。</span><span class="sxs-lookup"><span data-stu-id="1fcfc-104">Metadata for the given object.</span></span>

## <a name="properties"></a><span data-ttu-id="1fcfc-105">属性</span><span class="sxs-lookup"><span data-stu-id="1fcfc-105">Properties</span></span>
| <span data-ttu-id="1fcfc-106">属性</span><span class="sxs-lookup"><span data-stu-id="1fcfc-106">Property</span></span>     | <span data-ttu-id="1fcfc-107">类型</span><span class="sxs-lookup"><span data-stu-id="1fcfc-107">Type</span></span>   |<span data-ttu-id="1fcfc-108">说明</span><span class="sxs-lookup"><span data-stu-id="1fcfc-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1fcfc-109">Key</span><span class="sxs-lookup"><span data-stu-id="1fcfc-109">key</span></span>|<span data-ttu-id="1fcfc-110">String</span><span class="sxs-lookup"><span data-stu-id="1fcfc-110">String</span></span>|<span data-ttu-id="1fcfc-111">元数据属性的名称。</span><span class="sxs-lookup"><span data-stu-id="1fcfc-111">Name of the metadata property.</span></span>|
|<span data-ttu-id="1fcfc-112">value</span><span class="sxs-lookup"><span data-stu-id="1fcfc-112">value</span></span>|<span data-ttu-id="1fcfc-113">String</span><span class="sxs-lookup"><span data-stu-id="1fcfc-113">String</span></span>|<span data-ttu-id="1fcfc-114">元数据属性的值。</span><span class="sxs-lookup"><span data-stu-id="1fcfc-114">Value of the metadata property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1fcfc-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1fcfc-115">JSON representation</span></span>

<span data-ttu-id="1fcfc-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1fcfc-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.metadataEntry"
}-->

```json
{
  "key": "String",
  "value": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "metadataEntry resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-metadataentry.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
