---
title: timeZoneInformation 资源类型
description: 表示时区。 受支持的格式，Windows 和 Internet 分配号码证书颁发机构 (IANA) 时间区域 （也称为 Olson 时间区域）
ms.openlocfilehash: de80ed293af834d299be5f9543c5c3bedde7a540
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007720"
---
# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="6d6b8-104">timeZoneInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="6d6b8-104">timeZoneInformation resource type</span></span>


<span data-ttu-id="6d6b8-105">表示时区。</span><span class="sxs-lookup"><span data-stu-id="6d6b8-105">Represents a time zone.</span></span> <span data-ttu-id="6d6b8-106">支持的格式为 Windows，如果修复了当前已知问题，还支持 [Internet 编号分配机构 (IANA) 时区](https://www.iana.org/time-zones)（也称为 Olson 时区）格式。</span><span class="sxs-lookup"><span data-stu-id="6d6b8-106">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="6d6b8-107">属性</span><span class="sxs-lookup"><span data-stu-id="6d6b8-107">Properties</span></span>
| <span data-ttu-id="6d6b8-108">属性</span><span class="sxs-lookup"><span data-stu-id="6d6b8-108">Property</span></span>     | <span data-ttu-id="6d6b8-109">类型</span><span class="sxs-lookup"><span data-stu-id="6d6b8-109">Type</span></span>   |<span data-ttu-id="6d6b8-110">说明</span><span class="sxs-lookup"><span data-stu-id="6d6b8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d6b8-111">alias</span><span class="sxs-lookup"><span data-stu-id="6d6b8-111">alias</span></span>|<span data-ttu-id="6d6b8-112">string</span><span class="sxs-lookup"><span data-stu-id="6d6b8-112">string</span></span>|<span data-ttu-id="6d6b8-113">时区标识符。</span><span class="sxs-lookup"><span data-stu-id="6d6b8-113">An identifier for the time zone.</span></span>|
|<span data-ttu-id="6d6b8-114">displayName</span><span class="sxs-lookup"><span data-stu-id="6d6b8-114">displayName</span></span>|<span data-ttu-id="6d6b8-115">string</span><span class="sxs-lookup"><span data-stu-id="6d6b8-115">string</span></span>|<span data-ttu-id="6d6b8-116">表示时区的显示字符串。</span><span class="sxs-lookup"><span data-stu-id="6d6b8-116">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6d6b8-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6d6b8-117">JSON representation</span></span>

<span data-ttu-id="6d6b8-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d6b8-118">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "timeZoneInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->