---
title: deviceInstallState 资源类型
description: 包含某个设备的安装状态的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2b77d12e38816ae7621f8637720fa6cc0dfb46ed
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49295423"
---
# <a name="deviceinstallstate-resource-type"></a>deviceInstallState 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含某个设备的安装状态的属性。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[列出 deviceInstallStates](../api/intune-books-deviceinstallstate-list.md)|[deviceInstallState](../resources/intune-books-deviceinstallstate.md) 集合|列出 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性和关系。|
|[获取 deviceInstallState](../api/intune-books-deviceinstallstate-get.md)|[deviceInstallState](../resources/intune-books-deviceinstallstate.md)|读取 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性和关系。|
|[创建 deviceInstallState](../api/intune-books-deviceinstallstate-create.md)|[deviceInstallState](../resources/intune-books-deviceinstallstate.md)|创建新的 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象。|
|[删除 deviceInstallState](../api/intune-books-deviceinstallstate-delete.md)|无|删除 [deviceInstallState](../resources/intune-books-deviceinstallstate.md)。|
|[更新 deviceInstallState](../api/intune-books-deviceinstallstate-update.md)|[deviceInstallState](../resources/intune-books-deviceinstallstate.md)|更新 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|实体的键。|
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




