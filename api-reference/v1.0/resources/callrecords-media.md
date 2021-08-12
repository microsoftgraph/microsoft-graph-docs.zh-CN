---
title: 媒体资源类型
description: 媒体类型
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4e97d372e7c243a2cfbc4bbc8f44ec155a8addb70d624972a292ad9516824019
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54252114"
---
# <a name="media-resource-type"></a>媒体资源类型

命名空间：microsoft.graph.callRecords

表示用于 (音频、视频、基于视频的屏幕共享等) 媒体。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|标签|String|在媒体协商阶段如何标识媒体。|
|callerDevice|[microsoft.graph.callRecords.deviceInfo](callrecords-deviceinfo.md)|与此媒体的呼叫者终结点关联的设备信息。|
|callerNetwork|[microsoft.graph.callRecords.networkInfo](callrecords-networkinfo.md)|与此媒体的呼叫者终结点关联的网络信息。|
|calleeDevice|[microsoft.graph.callRecords.deviceInfo](callrecords-deviceinfo.md)|与此媒体的被叫方终结点关联的设备信息。|
|calleeNetwork|[microsoft.graph.callRecords.networkInfo](callrecords-networkinfo.md)|与此媒体的被叫方终结点关联的网络信息。|
|流|[microsoft.graph.callRecords.mediaStream](callrecords-mediastream.md) 集合|与此媒体关联的网络流。|

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
