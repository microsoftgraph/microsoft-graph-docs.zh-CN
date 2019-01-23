---
title: deviceInstallState 资源类型
description: 包含某个设备的安装状态的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c90b3e8e0693a28781a45f77cd00661528648439
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410719"
---
# <a name="deviceinstallstate-resource-type"></a>deviceInstallState 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含某个设备的安装状态的属性。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceInstallStates](../api/intune-books-deviceinstallstate-list.md)|[deviceInstallState](../resources/intune-books-deviceinstallstate.md) 集合|列出 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性和关系。|
|[获取 deviceInstallState](../api/intune-books-deviceinstallstate-get.md)|[deviceInstallState](../resources/intune-books-deviceinstallstate.md)|读取 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性和关系。|
|[创建 deviceInstallState](../api/intune-books-deviceinstallstate-create.md)|[deviceInstallState](../resources/intune-books-deviceinstallstate.md)|创建新的 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象。|
|[删除 deviceInstallState](../api/intune-books-deviceinstallstate-delete.md)|无|删除 [deviceInstallState](../resources/intune-books-deviceinstallstate.md)。|
|[更新 deviceInstallState](../api/intune-books-deviceinstallstate-update.md)|[deviceInstallState](../resources/intune-books-deviceinstallstate.md)|更新 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|deviceName|String|设备名称。|
|deviceId|String|设备 ID。|
|lastSyncDateTime|DateTimeOffset|上次同步日期和时间。|
|installState|[installState](../resources/intune-books-installstate.md)|电子图书的安装状态。 可取值为：`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown`。|
|errorCode|String|安装失败的错误代码。|
|osVersion|String|操作系统版本。|
|osDescription|String|操作系统说明。|
|userName|String|设备用户名。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceInstallState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "installState": "String",
  "errorCode": "String",
  "osVersion": "String",
  "osDescription": "String",
  "userName": "String"
}
```




