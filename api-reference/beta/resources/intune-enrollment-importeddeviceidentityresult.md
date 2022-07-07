---
title: importedDeviceIdentityResult 资源类型
description: importDeviceIdentityResult 资源表示尝试导入设备标识的结果。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9847091c9bd9c4ac39f9ac2b8db1428e04d3044e
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66666884"
---
# <a name="importeddeviceidentityresult-resource-type"></a>importedDeviceIdentityResult 资源类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

importDeviceIdentityResult 资源表示尝试导入设备标识的结果。


从 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) 继承

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 importedDeviceIdentityResults](../api/intune-enrollment-importeddeviceidentityresult-list.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) 集合|列出 [导入的DeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) 对象的属性和关系。|
|[获取 importedDeviceIdentityResult](../api/intune-enrollment-importeddeviceidentityresult-get.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|读取 [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) 对象的属性和关系。|
|[创建 importedDeviceIdentityResult](../api/intune-enrollment-importeddeviceidentityresult-create.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|创建新的 [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) 对象。|
|[删除 importedDeviceIdentityResult](../api/intune-enrollment-importeddeviceidentityresult-delete.md)|None|删除 [导入的DeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)。|
|[更新 importedDeviceIdentityResult](../api/intune-enrollment-importeddeviceidentityresult-update.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|更新 [导入的DeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|从导入的[DeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) 继承的导入设备标识的 ID|
|importedDeviceIdentifier|字符串|从[导入的DeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) 继承的导入设备标识符|
|importedDeviceIdentityType|[importedDeviceIdentityType](../resources/intune-enrollment-importeddeviceidentitytype.md)|从导入的 [DeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) 继承的导入设备标识的类型。 可取值为：`unknown`、`imei`、`serialNumber`。|
|lastModifiedDateTime|DateTimeOffset|从 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) 继承的说明的最后一个修改日期时间|
|createdDateTime|DateTimeOffset|从[导入的DeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) 继承的设备的创建日期时间|
|lastContactedDateTime|DateTimeOffset|从 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) 继承的设备的最后联系日期时间|
|说明|String|从导入的[DeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) 继承的设备的说明|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|Intune从[导入的DeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) 继承的设备状态。 可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。|
|平台|[平台](../resources/intune-enrollment-platform.md)|设备的平台。 继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。 可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。|
|status|Boolean|导入设备标识的状态|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedDeviceIdentityResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "id": "String (identifier)",
  "importedDeviceIdentifier": "String",
  "importedDeviceIdentityType": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String",
  "status": true
}
```




