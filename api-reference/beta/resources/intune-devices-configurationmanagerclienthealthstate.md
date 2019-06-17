---
title: configurationManagerClientHealthState 资源类型
description: 配置管理器客户端运行状况
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 618282f2a061ec8327ff93d1af441e088523260b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983237"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a>configurationManagerClientHealthState 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

配置管理器客户端运行状况

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|state|[configurationManagerClientState](../resources/intune-devices-configurationmanagerclientstate.md)|当前配置管理器客户端状态。 可取值为：`unknown`、`installed`、`healthy`、`installFailed`、`updateFailed`、`communicationError`。|
|errorCode|Int32|失败状态的错误代码。|
|lastSyncDateTime|DateTimeOffset|上次与 configuration manager 管理点同步的日期/时间。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientHealthState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientHealthState",
  "state": "String",
  "errorCode": 1024,
  "lastSyncDateTime": "String (timestamp)"
}
```





