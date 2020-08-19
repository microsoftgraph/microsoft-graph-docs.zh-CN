---
title: timeZoneInformation 资源类型
description: '表示时区。 受支持的格式为 Windows，并且 Internet 分配的号码颁发机构 (IANA) 时区 (也称为 Olson 时区) '
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 81f1eb3f8abbdcf95b94407019807d0d002dc286
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811824"
---
# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="6ed68-104">timeZoneInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="6ed68-104">timeZoneInformation resource type</span></span>

<span data-ttu-id="6ed68-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ed68-105">Namespace: microsoft.graph</span></span>


<span data-ttu-id="6ed68-106">表示时区。</span><span class="sxs-lookup"><span data-stu-id="6ed68-106">Represents a time zone.</span></span> <span data-ttu-id="6ed68-107">支持的格式为 Windows，如果修复了当前已知问题，还支持 [Internet 编号分配机构 (IANA) 时区](https://www.iana.org/time-zones)（也称为 Olson 时区）格式。</span><span class="sxs-lookup"><span data-stu-id="6ed68-107">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="6ed68-108">属性</span><span class="sxs-lookup"><span data-stu-id="6ed68-108">Properties</span></span>
| <span data-ttu-id="6ed68-109">属性</span><span class="sxs-lookup"><span data-stu-id="6ed68-109">Property</span></span>     | <span data-ttu-id="6ed68-110">类型</span><span class="sxs-lookup"><span data-stu-id="6ed68-110">Type</span></span>   |<span data-ttu-id="6ed68-111">说明</span><span class="sxs-lookup"><span data-stu-id="6ed68-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ed68-112">alias</span><span class="sxs-lookup"><span data-stu-id="6ed68-112">alias</span></span>|<span data-ttu-id="6ed68-113">string</span><span class="sxs-lookup"><span data-stu-id="6ed68-113">string</span></span>|<span data-ttu-id="6ed68-114">时区标识符。</span><span class="sxs-lookup"><span data-stu-id="6ed68-114">An identifier for the time zone.</span></span>|
|<span data-ttu-id="6ed68-115">displayName</span><span class="sxs-lookup"><span data-stu-id="6ed68-115">displayName</span></span>|<span data-ttu-id="6ed68-116">string</span><span class="sxs-lookup"><span data-stu-id="6ed68-116">string</span></span>|<span data-ttu-id="6ed68-117">表示时区的显示字符串。</span><span class="sxs-lookup"><span data-stu-id="6ed68-117">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6ed68-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ed68-118">JSON representation</span></span>

<span data-ttu-id="6ed68-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ed68-119">Here is a JSON representation of the resource.</span></span>

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
