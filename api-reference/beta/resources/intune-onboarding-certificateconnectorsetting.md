---
title: certificateConnectorSetting 资源类型
description: 证书连接器设置。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5886418aaddede43f2397ad626028598a63a0066
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398651"
---
# <a name="certificateconnectorsetting-resource-type"></a>certificateConnectorSetting 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

证书连接器设置。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|状态|Int32|证书连接器状态|
|certExpiryTime|DateTimeOffset|证书过期时间|
|enrollmentError|String|证书连接器注册错误|
|lastConnectorConnectionTime|DateTimeOffset|最后一次证书连接符连接|
|connectorVersion|String|证书连接器的版本|
|lastUploadVersion|Int64|版本的最后一个上载的证书连接器|

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




