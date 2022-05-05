---
title: zebraFotaConnector 资源类型
description: 表示租户的授权状态的 Zebra FOTA 连接器实体，供Intune调用 Zebra 更新服务。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ae01c91dc398f2780b4f0288233664c36ad7a8b4
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213163"
---
# <a name="zebrafotaconnector-resource-type"></a>zebraFotaConnector 资源类型

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示租户的授权状态的 Zebra FOTA 连接器实体，供Intune调用 Zebra 更新服务。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 zebraFotaConnector](../api/intune-androidfotaservice-zebrafotaconnector-get.md)|[zebraFotaConnector](../resources/intune-androidfotaservice-zebrafotaconnector.md)|读取 [zebraFotaConnector](../resources/intune-androidfotaservice-zebrafotaconnector.md) 对象的属性和关系。|
|[更新 zebraFotaConnector](../api/intune-androidfotaservice-zebrafotaconnector-update.md)|[zebraFotaConnector](../resources/intune-androidfotaservice-zebrafotaconnector.md)|更新 [zebraFotaConnector](../resources/intune-androidfotaservice-zebrafotaconnector.md) 对象的属性。|
|[hasActiveDeployments 操作](../api/intune-androidfotaservice-zebrafotaconnector-hasactivedeployments.md)|Boolean|尚未记录|
|[approveFotaApps 操作](../api/intune-androidfotaservice-zebrafotaconnector-approvefotaapps.md)|Boolean|尚未记录|
|[连接操作](../api/intune-androidfotaservice-zebrafotaconnector-connect.md)|Boolean|尚未记录|
|[断开连接操作](../api/intune-androidfotaservice-zebrafotaconnector-disconnect.md)|Boolean|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|ZebraFotaConnector 的 ID。|
|state|[zebraFotaConnectorState](../resources/intune-androidfotaservice-zebrafotaconnectorstate.md)|Zebra 连接器状态。 可能的值是：`none`、`connected`、`disconnected`、`unknownFutureValue`。|
|enrollmentToken|String|Zebra 的租户注册令牌。 该令牌用于通过应用配置在 FOTA 服务中注册 Zebra 设备。|
|enrollmentAuthorizationUrl|String|完成帐户注册授权 URL。 这与 Zebra API 文档中的verification_uri_complete相对应。|
|lastSyncDateTime|DateTimeOffset|帐户上次与 Zebra 同步的日期和时间|
|fotaAppsApproved|Boolean|指示是否已批准所需的固件无线 (FOTA) 应用的标志。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.zebraFotaConnector"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.zebraFotaConnector",
  "id": "String (identifier)",
  "state": "String",
  "enrollmentToken": "String",
  "enrollmentAuthorizationUrl": "String",
  "lastSyncDateTime": "String (timestamp)",
  "fotaAppsApproved": true
}
```




