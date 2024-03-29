---
title: traceRouteHop 资源类型
description: 表示为媒体流收集的网络跟踪路由跃点。
ms.localizationpriority: medium
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ed69c942e8d459ee9101a28d2243d842512c45d2
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436601"
---
# <a name="traceroutehop-resource-type"></a>traceRouteHop 资源类型

命名空间：microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示为 [媒体流](callrecords-mediastream.md)收集的网络跟踪路由跃点。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|hopCount|Int32|用于计算往返时间的此跃点的网络路径计数。|
|ipAddress|String|网络跟踪中用于此跃点的 IP 地址。|
|roundTripTime|期限|跟踪路由数据包从客户端发送到此跃点并返回到客户端的时间（以 [ISO 8601][] 格式表示）。 例如，1 秒表示为 `PT1S`P 是持续时间指定器，T 是时间指定器，S 是第二个指定器。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callRecords.traceRouteHop"
}-->

```json
{
  "hopCount": "Int32",
  "ipAddress": "String",
  "roundTripTime": "String (duration)"
}
```

[ISO 8601]: https://www.iso.org/iso/iso8601
