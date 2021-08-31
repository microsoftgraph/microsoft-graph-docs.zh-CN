---
title: unmanagedDevice 资源类型
description: 在网络中发现的非托管设备。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0286d1ac8790cff207ff754d49cd6d3ee51986de
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58806591"
---
# <a name="unmanageddevice-resource-type"></a>unmanagedDevice 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

在网络中发现的非托管设备。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|os|String|操作系统。|
|osVersion|String|操作系统版本。|
|ipAddress|String|IP 地址。|
|deviceName|String|设备名称。|
|macAddress|String|MAC 地址。|
|domain|字符串|域。|
|manufacturer|String|制造商。|
|model|String|模型。|
|位置|String|位置。|
|lastLoggedOnUser|String|上次登录的用户。|
|lastSeenDateTime|DateTimeOffset|上次看到日期和时间。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unmanagedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unmanagedDevice",
  "os": "String",
  "osVersion": "String",
  "ipAddress": "String",
  "deviceName": "String",
  "macAddress": "String",
  "domain": "String",
  "manufacturer": "String",
  "model": "String",
  "location": "String",
  "lastLoggedOnUser": "String",
  "lastSeenDateTime": "String (timestamp)"
}
```



