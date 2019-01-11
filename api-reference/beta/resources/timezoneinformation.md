---
title: timeZoneInformation 资源类型
description: 表示时区。 受支持的格式，Windows 和 Internet 分配号码证书颁发机构 (IANA) 时间区域 （也称为 Olson 时间区域）
localization_priority: Normal
ms.openlocfilehash: dc53cca34ef9c6a53a39394cbba8be4e1baca662
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839737"
---
# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="170d3-104">timeZoneInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="170d3-104">timeZoneInformation resource type</span></span>

> <span data-ttu-id="170d3-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="170d3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="170d3-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="170d3-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="170d3-107">表示时区。</span><span class="sxs-lookup"><span data-stu-id="170d3-107">Represents a time zone.</span></span> <span data-ttu-id="170d3-108">支持的格式为 Windows，如果修复了当前已知问题，还支持 [Internet 编号分配机构 (IANA) 时区](https://www.iana.org/time-zones)（也称为 Olson 时区）格式。</span><span class="sxs-lookup"><span data-stu-id="170d3-108">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="170d3-109">属性</span><span class="sxs-lookup"><span data-stu-id="170d3-109">Properties</span></span>
| <span data-ttu-id="170d3-110">属性</span><span class="sxs-lookup"><span data-stu-id="170d3-110">Property</span></span>     | <span data-ttu-id="170d3-111">类型</span><span class="sxs-lookup"><span data-stu-id="170d3-111">Type</span></span>   |<span data-ttu-id="170d3-112">说明</span><span class="sxs-lookup"><span data-stu-id="170d3-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="170d3-113">alias</span><span class="sxs-lookup"><span data-stu-id="170d3-113">alias</span></span>|<span data-ttu-id="170d3-114">string</span><span class="sxs-lookup"><span data-stu-id="170d3-114">string</span></span>|<span data-ttu-id="170d3-115">时区标识符。</span><span class="sxs-lookup"><span data-stu-id="170d3-115">An identifier for the time zone.</span></span>|
|<span data-ttu-id="170d3-116">displayName</span><span class="sxs-lookup"><span data-stu-id="170d3-116">displayName</span></span>|<span data-ttu-id="170d3-117">string</span><span class="sxs-lookup"><span data-stu-id="170d3-117">string</span></span>|<span data-ttu-id="170d3-118">表示时区的显示字符串。</span><span class="sxs-lookup"><span data-stu-id="170d3-118">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="170d3-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="170d3-119">JSON representation</span></span>

<span data-ttu-id="170d3-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="170d3-120">Here is a JSON representation of the resource.</span></span>

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
