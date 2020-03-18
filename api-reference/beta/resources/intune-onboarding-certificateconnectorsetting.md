---
title: certificateConnectorSetting 资源类型
description: 证书连接器设置。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3230a5b512ab09b8b3c033f95c3fc7682197ff4a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42779875"
---
# <a name="certificateconnectorsetting-resource-type"></a>certificateConnectorSetting 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

证书连接器设置。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|状态|Int32|证书连接器状态|
|certExpiryTime|DateTimeOffset|证书过期时间|
|enrollmentError|String|证书连接器注册错误|
|lastConnectorConnectionTime|DateTimeOffset|上次连接证书连接器的时间|
|connectorVersion|String|证书连接器的版本|
|lastUploadVersion|Int64|上次上载的证书连接器的版本|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.certificateConnectorSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.certificateConnectorSetting",
  "status": 1024,
  "certExpiryTime": "String (timestamp)",
  "enrollmentError": "String",
  "lastConnectorConnectionTime": "String (timestamp)",
  "connectorVersion": "String",
  "lastUploadVersion": 1024
}
```



