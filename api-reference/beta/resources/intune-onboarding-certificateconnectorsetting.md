---
title: certificateConnectorSetting 资源类型
description: 证书连接器设置。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 56f12600b6aa78982dc51732d685dcd7c962d0b0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888597"
---
# <a name="certificateconnectorsetting-resource-type"></a>certificateConnectorSetting 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

证书连接器设置。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|状态|Int32|证书连接器状态|
|certExpiryTime|DateTimeOffset|证书过期时间|
|enrollmentError|字符串|证书连接器注册错误|
|lastConnectorConnectionTime|DateTimeOffset|最后一次证书连接符连接|
|connectorVersion|字符串|证书连接器的版本|
|lastUploadVersion|Int64|版本的最后一个上载的证书连接器|

## <a name="relationships"></a>Relationships
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





