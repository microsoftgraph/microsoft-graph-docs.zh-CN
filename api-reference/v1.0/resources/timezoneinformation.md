---
title: timeZoneInformation 资源类型
description: 表示时区。 受支持的格式为 Windows, Internet 分配的号码颁发机构 (IANA) 时区 (也称为 "Olson 时区")
localization_priority: Normal
ms.openlocfilehash: ced18a28a5c086416fa7247e1531d772fd63b977
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456911"
---
# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="f0270-104">timeZoneInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="f0270-104">timeZoneInformation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0270-105">表示时区。</span><span class="sxs-lookup"><span data-stu-id="f0270-105">Represents a time zone.</span></span> <span data-ttu-id="f0270-106">支持的格式为 Windows，如果修复了当前已知问题，还支持 [Internet 编号分配机构 (IANA) 时区](https://www.iana.org/time-zones)（也称为 Olson 时区）格式。</span><span class="sxs-lookup"><span data-stu-id="f0270-106">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="f0270-107">属性</span><span class="sxs-lookup"><span data-stu-id="f0270-107">Properties</span></span>
| <span data-ttu-id="f0270-108">属性</span><span class="sxs-lookup"><span data-stu-id="f0270-108">Property</span></span>     | <span data-ttu-id="f0270-109">类型</span><span class="sxs-lookup"><span data-stu-id="f0270-109">Type</span></span>   |<span data-ttu-id="f0270-110">说明</span><span class="sxs-lookup"><span data-stu-id="f0270-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0270-111">alias</span><span class="sxs-lookup"><span data-stu-id="f0270-111">alias</span></span>|<span data-ttu-id="f0270-112">string</span><span class="sxs-lookup"><span data-stu-id="f0270-112">string</span></span>|<span data-ttu-id="f0270-113">时区标识符。</span><span class="sxs-lookup"><span data-stu-id="f0270-113">An identifier for the time zone.</span></span>|
|<span data-ttu-id="f0270-114">displayName</span><span class="sxs-lookup"><span data-stu-id="f0270-114">displayName</span></span>|<span data-ttu-id="f0270-115">string</span><span class="sxs-lookup"><span data-stu-id="f0270-115">string</span></span>|<span data-ttu-id="f0270-116">表示时区的显示字符串。</span><span class="sxs-lookup"><span data-stu-id="f0270-116">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f0270-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0270-117">JSON representation</span></span>

<span data-ttu-id="f0270-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0270-118">Here is a JSON representation of the resource.</span></span>

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
