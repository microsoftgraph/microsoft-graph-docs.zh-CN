---
title: timeZoneInformation 资源类型
description: 表示时区。 受支持的格式，Windows 和 Internet 分配号码证书颁发机构 (IANA) 时间区域 （也称为 Olson 时间区域）
localization_priority: Normal
ms.openlocfilehash: a63721de7ed4e8c3f3b74ce5954a88ee71a95414
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526772"
---
# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="f8825-104">timeZoneInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="f8825-104">timeZoneInformation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8825-105">表示时区。</span><span class="sxs-lookup"><span data-stu-id="f8825-105">Represents a time zone.</span></span> <span data-ttu-id="f8825-106">支持的格式为 Windows，如果修复了当前已知问题，还支持 [Internet 编号分配机构 (IANA) 时区](https://www.iana.org/time-zones)（也称为 Olson 时区）格式。</span><span class="sxs-lookup"><span data-stu-id="f8825-106">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="f8825-107">属性</span><span class="sxs-lookup"><span data-stu-id="f8825-107">Properties</span></span>
| <span data-ttu-id="f8825-108">属性</span><span class="sxs-lookup"><span data-stu-id="f8825-108">Property</span></span>     | <span data-ttu-id="f8825-109">类型</span><span class="sxs-lookup"><span data-stu-id="f8825-109">Type</span></span>   |<span data-ttu-id="f8825-110">说明</span><span class="sxs-lookup"><span data-stu-id="f8825-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f8825-111">alias</span><span class="sxs-lookup"><span data-stu-id="f8825-111">alias</span></span>|<span data-ttu-id="f8825-112">string</span><span class="sxs-lookup"><span data-stu-id="f8825-112">string</span></span>|<span data-ttu-id="f8825-113">时区标识符。</span><span class="sxs-lookup"><span data-stu-id="f8825-113">An identifier for the time zone.</span></span>|
|<span data-ttu-id="f8825-114">displayName</span><span class="sxs-lookup"><span data-stu-id="f8825-114">displayName</span></span>|<span data-ttu-id="f8825-115">string</span><span class="sxs-lookup"><span data-stu-id="f8825-115">string</span></span>|<span data-ttu-id="f8825-116">表示时区的显示字符串。</span><span class="sxs-lookup"><span data-stu-id="f8825-116">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f8825-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f8825-117">JSON representation</span></span>

<span data-ttu-id="f8825-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f8825-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneInformation"
}-->

```json
{
  "alias": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeZoneInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timezoneinformation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
