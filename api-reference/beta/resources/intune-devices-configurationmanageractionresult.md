---
title: configurationManagerActionResult 资源类型
description: ConfigurationManager 操作的结果
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9fbe2827194403c8295e9ef59a1089c698f14092
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611977"
---
# <a name="configurationmanageractionresult-resource-type"></a>configurationManagerActionResult 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

ConfigurationManager 操作的结果


继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|actionName|String|操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)|
|actionState|[actionState](../resources/intune-devices-actionstate.md)|操作的状态 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)。 可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。|
|startDateTime|DateTimeOffset|操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)|
|lastUpdatedDateTime|DateTimeOffset|操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)|
|actionDeliveryStatus|[configurationManagerActionDeliveryStatus](../resources/intune-devices-configurationmanageractiondeliverystatus.md)|要传递到场服务器的操作的状态。 可取值为：`unknown`、`pendingDelivery`、`deliveredToConnectorService`、`failedToDeliverToConnectorService`、`deliveredToOnPremisesServer`。|
|errorCode|Int32|来自客户端的配置管理器操作的错误代码|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "actionDeliveryStatus": "String",
  "errorCode": 1024
}
```




