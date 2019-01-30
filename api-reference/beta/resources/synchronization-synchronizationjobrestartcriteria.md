---
title: synchronizationJobRestartCriteria 资源类型
description: 定义的范围的[synchronizationJob： 重新启动](../api/synchronization_synchronizationjob_restart.md)操作。
localization_priority: Normal
ms.openlocfilehash: 1e6ac952808f80d191fc93e9a804411ec4459d4c
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642518"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a><span data-ttu-id="a37ed-103">synchronizationJobRestartCriteria 资源类型</span><span class="sxs-lookup"><span data-stu-id="a37ed-103">synchronizationJobRestartCriteria resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a37ed-104">定义的范围的[synchronizationJob： 重新启动](../api/synchronization_synchronizationjob_restart.md)操作。</span><span class="sxs-lookup"><span data-stu-id="a37ed-104">Defines the scope of the [synchronizationJob: restart](../api/synchronization_synchronizationjob_restart.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="a37ed-105">属性</span><span class="sxs-lookup"><span data-stu-id="a37ed-105">Properties</span></span>
| <span data-ttu-id="a37ed-106">属性</span><span class="sxs-lookup"><span data-stu-id="a37ed-106">Property</span></span>     | <span data-ttu-id="a37ed-107">类型</span><span class="sxs-lookup"><span data-stu-id="a37ed-107">Type</span></span>   |<span data-ttu-id="a37ed-108">说明</span><span class="sxs-lookup"><span data-stu-id="a37ed-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a37ed-109">resetScope</span><span class="sxs-lookup"><span data-stu-id="a37ed-109">resetScope</span></span>|<span data-ttu-id="a37ed-110">String</span><span class="sxs-lookup"><span data-stu-id="a37ed-110">String</span></span>| <span data-ttu-id="a37ed-111">以逗号分隔的下列值的组合： `Full`， `QuarantineState`， `Watermark`， `Escrows`， `ConnectorDataStore`。</span><span class="sxs-lookup"><span data-stu-id="a37ed-111">Comma-separated combination of the following values: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span></span> <span data-ttu-id="a37ed-112">使用`Full`如果希望所有选项。</span><span class="sxs-lookup"><span data-stu-id="a37ed-112">Use `Full` if you want all of the options.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a37ed-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a37ed-113">JSON representation</span></span>

<span data-ttu-id="a37ed-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a37ed-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationJobRestartCriteria"
}-->

```json
{
  "resetScope": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJobRestartCriteria resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationjobrestartcriteria.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
