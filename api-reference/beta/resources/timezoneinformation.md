---
title: timeZoneInformation 资源类型
description: '表示时区。 受支持的格式为 Windows，并且 Internet 分配的号码颁发机构 (IANA) 时区 (也称为 Olson 时区) '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3deae74f1ffc991e6e9178a46575c21d69272d2c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519678"
---
# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="87051-104">timeZoneInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="87051-104">timeZoneInformation resource type</span></span>

<span data-ttu-id="87051-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87051-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87051-106">表示时区。</span><span class="sxs-lookup"><span data-stu-id="87051-106">Represents a time zone.</span></span> <span data-ttu-id="87051-107">支持的格式为 Windows，如果修复了当前已知问题，还支持 [Internet 编号分配机构 (IANA) 时区](https://www.iana.org/time-zones)（也称为 Olson 时区）格式。</span><span class="sxs-lookup"><span data-stu-id="87051-107">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="87051-108">属性</span><span class="sxs-lookup"><span data-stu-id="87051-108">Properties</span></span>
| <span data-ttu-id="87051-109">属性</span><span class="sxs-lookup"><span data-stu-id="87051-109">Property</span></span>     | <span data-ttu-id="87051-110">类型</span><span class="sxs-lookup"><span data-stu-id="87051-110">Type</span></span>   |<span data-ttu-id="87051-111">说明</span><span class="sxs-lookup"><span data-stu-id="87051-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="87051-112">alias</span><span class="sxs-lookup"><span data-stu-id="87051-112">alias</span></span>|<span data-ttu-id="87051-113">string</span><span class="sxs-lookup"><span data-stu-id="87051-113">string</span></span>|<span data-ttu-id="87051-114">时区标识符。</span><span class="sxs-lookup"><span data-stu-id="87051-114">An identifier for the time zone.</span></span>|
|<span data-ttu-id="87051-115">displayName</span><span class="sxs-lookup"><span data-stu-id="87051-115">displayName</span></span>|<span data-ttu-id="87051-116">string</span><span class="sxs-lookup"><span data-stu-id="87051-116">string</span></span>|<span data-ttu-id="87051-117">表示时区的显示字符串。</span><span class="sxs-lookup"><span data-stu-id="87051-117">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="87051-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="87051-118">JSON representation</span></span>

<span data-ttu-id="87051-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="87051-119">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
