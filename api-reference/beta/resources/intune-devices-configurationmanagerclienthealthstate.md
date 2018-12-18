---
title: configurationManagerClientHealthState 资源类型
description: 配置管理器客户端健康状态
author: tfitzmac
ms.openlocfilehash: 8361d74f675cf1eaf70b78e2350aae2fc6e83554
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302784"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a>configurationManagerClientHealthState 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

配置管理器客户端健康状态
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|state|[configurationManagerClientState](../resources/intune-devices-configurationmanagerclientstate.md)|当前配置管理器客户端状态。 可取值为：`unknown`、`installed`、`healthy`、`installFailed`、`updateFailed`、`communicationError`。|
|errorCode|Int32|失败的状态的错误代码。|
|lastSyncDateTime|DateTimeOffset|指向与配置管理器管理的 Datetime fo 上次同步。|

## <a name="relationships"></a>Relationships
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





