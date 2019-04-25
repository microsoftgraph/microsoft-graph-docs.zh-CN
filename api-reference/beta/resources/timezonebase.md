---
title: timeZoneBase 资源类型
description: 时区的基本表示形式。
localization_priority: Normal
ms.openlocfilehash: 9fc07961aaa475980309d8c843b613da8b42e448
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523012"
---
# <a name="timezonebase-resource-type"></a><span data-ttu-id="9ebb4-103">timeZoneBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="9ebb4-103">timeZoneBase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ebb4-104">时区的基本表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ebb4-104">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="9ebb4-105">属性</span><span class="sxs-lookup"><span data-stu-id="9ebb4-105">Properties</span></span>
| <span data-ttu-id="9ebb4-106">属性</span><span class="sxs-lookup"><span data-stu-id="9ebb4-106">Property</span></span>     | <span data-ttu-id="9ebb4-107">类型</span><span class="sxs-lookup"><span data-stu-id="9ebb4-107">Type</span></span>   |<span data-ttu-id="9ebb4-108">说明</span><span class="sxs-lookup"><span data-stu-id="9ebb4-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9ebb4-109">name</span><span class="sxs-lookup"><span data-stu-id="9ebb4-109">name</span></span> | <span data-ttu-id="9ebb4-110">string</span><span class="sxs-lookup"><span data-stu-id="9ebb4-110">string</span></span> | <span data-ttu-id="9ebb4-111">时区的名称。</span><span class="sxs-lookup"><span data-stu-id="9ebb4-111">The name of a time zone.</span></span> <span data-ttu-id="9ebb4-112">它可以是一个标准时区名称，例如“夏威夷-阿留申标准时间”，或自定义时区的“自定义时区”。</span><span class="sxs-lookup"><span data-stu-id="9ebb4-112">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="9ebb4-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9ebb4-113">JSON representation</span></span>

<span data-ttu-id="9ebb4-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ebb4-114">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneBase"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeZoneBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timezonebase.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
