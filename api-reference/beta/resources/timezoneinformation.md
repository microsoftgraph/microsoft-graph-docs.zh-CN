---
title: timeZoneInformation 资源类型
description: 表示时区。 受支持的格式，Windows 和 Internet 分配号码证书颁发机构 (IANA) 时间区域 （也称为 Olson 时间区域）
ms.openlocfilehash: 5508f20812b8327a068364df7eb33c5072c3512e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045003"
---
# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="4ed80-104">timeZoneInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="4ed80-104">timeZoneInformation resource type</span></span>

> <span data-ttu-id="4ed80-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4ed80-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ed80-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4ed80-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4ed80-107">表示时区。</span><span class="sxs-lookup"><span data-stu-id="4ed80-107">Represents a time zone.</span></span> <span data-ttu-id="4ed80-108">支持的格式为 Windows，如果修复了当前已知问题，还支持 [Internet 编号分配机构 (IANA) 时区](https://www.iana.org/time-zones)（也称为 Olson 时区）格式。</span><span class="sxs-lookup"><span data-stu-id="4ed80-108">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="4ed80-109">属性</span><span class="sxs-lookup"><span data-stu-id="4ed80-109">Properties</span></span>
| <span data-ttu-id="4ed80-110">属性</span><span class="sxs-lookup"><span data-stu-id="4ed80-110">Property</span></span>     | <span data-ttu-id="4ed80-111">类型</span><span class="sxs-lookup"><span data-stu-id="4ed80-111">Type</span></span>   |<span data-ttu-id="4ed80-112">说明</span><span class="sxs-lookup"><span data-stu-id="4ed80-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ed80-113">alias</span><span class="sxs-lookup"><span data-stu-id="4ed80-113">alias</span></span>|<span data-ttu-id="4ed80-114">string</span><span class="sxs-lookup"><span data-stu-id="4ed80-114">string</span></span>|<span data-ttu-id="4ed80-115">时区标识符。</span><span class="sxs-lookup"><span data-stu-id="4ed80-115">An identifier for the time zone.</span></span>|
|<span data-ttu-id="4ed80-116">displayName</span><span class="sxs-lookup"><span data-stu-id="4ed80-116">displayName</span></span>|<span data-ttu-id="4ed80-117">string</span><span class="sxs-lookup"><span data-stu-id="4ed80-117">string</span></span>|<span data-ttu-id="4ed80-118">表示时区的显示字符串。</span><span class="sxs-lookup"><span data-stu-id="4ed80-118">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4ed80-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4ed80-119">JSON representation</span></span>

<span data-ttu-id="4ed80-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ed80-120">Here is a JSON representation of the resource.</span></span>

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