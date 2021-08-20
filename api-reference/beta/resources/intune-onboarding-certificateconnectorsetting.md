---
title: certificateConnectorSetting 资源类型
description: 证书连接器设置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 31b8ec7fcfe95e459e6454635b7b5e0a37c16cdec45eba5515a24165ad5ad80d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54206247"
---
# <a name="certificateconnectorsetting-resource-type"></a>certificateConnectorSetting 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

证书连接器设置。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|状态|Int32|证书连接器状态|
|certExpiryTime|DateTimeOffset|证书过期时间|
|enrollmentError|字符串|证书连接器注册错误|
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




