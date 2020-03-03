---
title: 媒体资源类型
description: 媒体类型
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 1b996c34c3d12984cc512dbcc4d1113d54bd5f69
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394700"
---
# <a name="media-resource-type"></a>媒体资源类型

命名空间： callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在呼叫中使用的媒体（音频、视频、基于视频的屏幕共享等）。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|label|String|媒体在媒体协商阶段中的标识方式。|
|callerDevice|[callRecords。 deviceInfo](callrecords-deviceinfo.md)|与此媒体的呼叫方终结点关联的设备信息。|
|callerNetwork|[callRecords。 networkInfo](callrecords-networkinfo.md)|与此媒体的呼叫方终结点关联的网络信息。|
|calleeDevice|[callRecords。 deviceInfo](callrecords-deviceinfo.md)|与此媒体的被呼叫者终结点关联的设备信息。|
|calleeNetwork|[callRecords。 networkInfo](callrecords-networkinfo.md)|与此媒体的被呼叫者终结点关联的网络信息。|
|连续流|[callRecords](callrecords-mediastream.md)集合的 mediaStream|与此媒体关联的网络流。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.media",
  "baseType": null
}-->

```json
{
  "label": "String",
  "callerDevice": {"@odata.type": "microsoft.graph.callRecords.deviceInfo"},
  "callerNetwork": {"@odata.type": "microsoft.graph.callRecords.networkInfo"},
  "calleeDevice": {"@odata.type": "microsoft.graph.callRecords.deviceInfo"},
  "calleeNetwork": {"@odata.type": "microsoft.graph.callRecords.networkInfo"},
  "streams": [{"@odata.type": "microsoft.graph.callRecords.mediaStream"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "media resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->