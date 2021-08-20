---
title: windowsManagementAppHealthState 资源类型
description: Windows管理应用运行状况状态实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b5cd8230391f904e3a16218ec213ea8111158b4e9234fd47ec6878b8d3461b3b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54227349"
---
# <a name="windowsmanagementapphealthstate-resource-type"></a>windowsManagementAppHealthState 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows管理应用运行状况状态实体。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsManagementAppHealthStates](../api/intune-devices-windowsmanagementapphealthstate-list.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) 集合|列出 [windowsManagementAppHealthState 对象的属性和](../resources/intune-devices-windowsmanagementapphealthstate.md) 关系。|
|[获取 windowsManagementAppHealthState](../api/intune-devices-windowsmanagementapphealthstate-get.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|读取 [windowsManagementAppHealthState 对象的属性和](../resources/intune-devices-windowsmanagementapphealthstate.md) 关系。|
|[创建 windowsManagementAppHealthState](../api/intune-devices-windowsmanagementapphealthstate-create.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|创建新的 [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) 对象。|
|[删除 windowsManagementAppHealthState](../api/intune-devices-windowsmanagementapphealthstate-delete.md)|无|删除 [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)。|
|[更新 windowsManagementAppHealthState](../api/intune-devices-windowsmanagementapphealthstate-update.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|更新 [windowsManagementAppHealthState 对象](../resources/intune-devices-windowsmanagementapphealthstate.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|管理应用Windows状态的唯一标识符。 此属性是只读的。|
|healthState|[healthState](../resources/intune-devices-healthstate.md)|Windows管理应用运行状况状态。 可取值为：`unknown`、`healthy`、`unhealthy`。|
|installedVersion|字符串|Windows管理应用安装的版本。|
|lastCheckInDateTime|DateTimeOffset|Windows管理应用上次签入时间。|
|deviceName|String|安装了管理应用Windows的名称。|
|deviceOSVersion|String|Windows 10安装了管理应用Windows操作系统版本。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementAppHealthState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "id": "String (identifier)",
  "healthState": "String",
  "installedVersion": "String",
  "lastCheckInDateTime": "String (timestamp)",
  "deviceName": "String",
  "deviceOSVersion": "String"
}
```




