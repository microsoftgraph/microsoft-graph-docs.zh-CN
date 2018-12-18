---
title: windowsManagementAppHealthState 资源类型
description: Windows 管理应用程序运行状况状态实体。
author: tfitzmac
ms.openlocfilehash: 5ff77ce54a99ed71a8f4b3498a469342b2e46367
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359701"
---
# <a name="windowsmanagementapphealthstate-resource-type"></a>windowsManagementAppHealthState 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Windows 管理应用程序运行状况状态实体。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 windowsManagementAppHealthStates](../api/intune-devices-windowsmanagementapphealthstate-list.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)集合|列出属性和[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象之间的关系。|
|[获取 windowsManagementAppHealthState](../api/intune-devices-windowsmanagementapphealthstate-get.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|读取属性和[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象的关系。|
|[创建 windowsManagementAppHealthState](../api/intune-devices-windowsmanagementapphealthstate-create.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|创建新的[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象。|
|[删除 windowsManagementAppHealthState](../api/intune-devices-windowsmanagementapphealthstate-delete.md)|无|删除[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)。|
|[更新 windowsManagementAppHealthState](../api/intune-devices-windowsmanagementapphealthstate-update.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|更新[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|Windows 管理应用程序的运行状况状态的唯一标识符|
|healthState|[healthState](../resources/intune-devices-healthstate.md)|Windows 管理应用程序的运行状况状态。 可取值为：`unknown`、`healthy`、`unhealthy`。|
|installedVersion|字符串|Windows 管理应用程序安装的版本。|
|lastCheckInDateTime|DateTimeOffset|Windows 管理应用程序上次签入的时间。|
|deviceName|String|设备的 Windows 安装管理应用程序的名称。|
|deviceOSVersion|字符串|Windows 10 OS 版本的 Windows 安装管理应用程序的设备。|

## <a name="relationships"></a>Relationships
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





