---
title: importedDeviceIdentityResult 资源类型
description: importedDeviceIdentityResult 资源表示尝试导入设备标识的结果。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b94eff5ea5e2ed37173341b45980e9b60437822d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524496"
---
# <a name="importeddeviceidentityresult-resource-type"></a>importedDeviceIdentityResult 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

importedDeviceIdentityResult 资源表示尝试导入设备标识的结果。


继承自[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 importedDeviceIdentityResults](../api/intune-enrollment-importeddeviceidentityresult-list.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)集合|列出[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)对象的属性和关系。|
|[获取 importedDeviceIdentityResult](../api/intune-enrollment-importeddeviceidentityresult-get.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|读取[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)对象的属性和关系。|
|[创建 importedDeviceIdentityResult](../api/intune-enrollment-importeddeviceidentityresult-create.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|创建新的[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)对象。|
|[删除 importedDeviceIdentityResult](../api/intune-enrollment-importeddeviceidentityresult-delete.md)|无|删除[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)。|
|[更新 importedDeviceIdentityResult](../api/intune-enrollment-importeddeviceidentityresult-update.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|更新[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|从[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的导入设备标识的 Id|
|importedDeviceIdentifier|String|从[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的导入设备标识符|
|importedDeviceIdentityType|[importedDeviceIdentityType](../resources/intune-enrollment-importeddeviceidentitytype.md)|从[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的导入设备标识的类型。 可取值为：`unknown`、`imei`、`serialNumber`。|
|lastModifiedDateTime|DateTimeOffset|继承自[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)的说明的上次修改日期时间|
|createdDateTime|DateTimeOffset|从[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的设备的创建日期时间|
|lastContactedDateTime|DateTimeOffset|从[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的设备的上次联系日期时间|
|description|String|从[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)继承的设备的说明|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|Intune 中的设备的状态继承自[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。 可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。|
|platform|[平台](../resources/intune-enrollment-platform.md)|设备的平台。 继承自[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。 可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。|
|状态|布尔值|导入的设备标识的状态|

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





