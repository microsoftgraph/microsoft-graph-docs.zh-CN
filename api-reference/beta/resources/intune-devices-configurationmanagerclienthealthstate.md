---
title: configurationManagerClientHealthState 资源类型
description: 配置管理器客户端健康状态
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 55ba2b24df0d1d4c278f4785a310237c9c32cd9b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425825"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a>configurationManagerClientHealthState 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

配置管理器客户端健康状态

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|state|[configurationManagerClientState](../resources/intune-devices-configurationmanagerclientstate.md)|当前配置管理器客户端状态。 可取值为：`unknown`、`installed`、`healthy`、`installFailed`、`updateFailed`、`communicationError`。|
|errorCode|Int32|失败的状态的错误代码。|
|lastSyncDateTime|DateTimeOffset|指向与配置管理器管理的 Datetime fo 上次同步。|

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




