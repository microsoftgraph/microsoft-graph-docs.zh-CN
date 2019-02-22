---
title: certificateConnectorSetting 资源类型
description: 证书连接器设置。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 09f4baf9ddd8be630c432fcec5d7df71c442bbe2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168304"
---
# <a name="certificateconnectorsetting-resource-type"></a>certificateConnectorSetting 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

证书连接器设置。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|状态|Int32|证书连接器状态|
|certExpiryTime|DateTimeOffset|证书过期时间|
|enrollmentError|字符串|证书连接器注册错误|
|lastConnectorConnectionTime|DateTimeOffset|上次连接证书连接器的时间|
|connectorVersion|字符串|证书连接器的版本|
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




