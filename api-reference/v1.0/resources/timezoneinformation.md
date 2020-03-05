---
title: timeZoneInformation 资源类型
description: 表示时区。 受支持的格式为 Windows，Internet 分配的号码颁发机构（IANA）时区（也称为 "Olson 时区"）
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 2b09e95db4c6d599e1e61925991912bb55ff8424
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446805"
---
# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="0622e-104">timeZoneInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="0622e-104">timeZoneInformation resource type</span></span>

<span data-ttu-id="0622e-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0622e-105">Namespace: microsoft.graph</span></span>


<span data-ttu-id="0622e-106">表示时区。</span><span class="sxs-lookup"><span data-stu-id="0622e-106">Represents a time zone.</span></span> <span data-ttu-id="0622e-107">支持的格式为 Windows，如果修复了当前已知问题，还支持 [Internet 编号分配机构 (IANA) 时区](https://www.iana.org/time-zones)（也称为 Olson 时区）格式。</span><span class="sxs-lookup"><span data-stu-id="0622e-107">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="0622e-108">属性</span><span class="sxs-lookup"><span data-stu-id="0622e-108">Properties</span></span>
| <span data-ttu-id="0622e-109">属性</span><span class="sxs-lookup"><span data-stu-id="0622e-109">Property</span></span>     | <span data-ttu-id="0622e-110">类型</span><span class="sxs-lookup"><span data-stu-id="0622e-110">Type</span></span>   |<span data-ttu-id="0622e-111">说明</span><span class="sxs-lookup"><span data-stu-id="0622e-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0622e-112">alias</span><span class="sxs-lookup"><span data-stu-id="0622e-112">alias</span></span>|<span data-ttu-id="0622e-113">string</span><span class="sxs-lookup"><span data-stu-id="0622e-113">string</span></span>|<span data-ttu-id="0622e-114">时区标识符。</span><span class="sxs-lookup"><span data-stu-id="0622e-114">An identifier for the time zone.</span></span>|
|<span data-ttu-id="0622e-115">displayName</span><span class="sxs-lookup"><span data-stu-id="0622e-115">displayName</span></span>|<span data-ttu-id="0622e-116">string</span><span class="sxs-lookup"><span data-stu-id="0622e-116">string</span></span>|<span data-ttu-id="0622e-117">表示时区的显示字符串。</span><span class="sxs-lookup"><span data-stu-id="0622e-117">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0622e-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0622e-118">JSON representation</span></span>

<span data-ttu-id="0622e-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0622e-119">Here is a JSON representation of the resource.</span></span>

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
