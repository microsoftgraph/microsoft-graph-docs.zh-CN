---
title: certificateConnectorSetting 资源类型
description: 证书连接器设置。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fd809fd2cb26a57d13ad7a4c250868b44967020a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967754"
---
# <a name="certificateconnectorsetting-resource-type"></a>certificateConnectorSetting 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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





