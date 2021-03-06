---
title: windowsManagementApp 资源类型
description: Windows管理应用实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 540ba41779e64c57b5c74c7acf004172a1567c37
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665572"
---
# <a name="windowsmanagementapp-resource-type"></a>windowsManagementApp 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows管理应用实体。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 windowsManagementApp](../api/intune-devices-windowsmanagementapp-get.md)|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)|读取 [windowsManagementApp 对象的属性和](../resources/intune-devices-windowsmanagementapp.md) 关系。|
|[更新 windowsManagementApp](../api/intune-devices-windowsmanagementapp-update.md)|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)|更新 [windowsManagementApp 对象](../resources/intune-devices-windowsmanagementapp.md) 的属性。|
|[setAsManagedInstaller 操作](../api/intune-devices-windowsmanagementapp-setasmanagedinstaller.md)|无|设置呼叫者租户的托管安装程序状态|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|管理应用程序的唯Windows标识符|
|availableVersion|String|Windows管理应用可用版本。|
|managedInstaller|[managedInstallerStatus](../resources/intune-devices-managedinstallerstatus.md)|托管安装程序状态。 可取值为：`disabled`、`enabled`。|
|managedInstallerConfiguredDateTime|String|托管安装程序配置的日期时间|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|healthStates|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) 集合|已安装的运行状况状态列表Windows管理应用。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "String (identifier)",
  "availableVersion": "String",
  "managedInstaller": "String",
  "managedInstallerConfiguredDateTime": "String"
}
```




