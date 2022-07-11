---
title: importedDeviceIdentity 资源类型
description: 导入的DeviceIdentity 资源表示为预注册配置预暂存的设备的唯一硬件标识。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 19da44719f1e7f72358350509eec6c52aaeff122
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66667262"
---
# <a name="importeddeviceidentity-resource-type"></a>importedDeviceIdentity 资源类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

导入的DeviceIdentity 资源表示为预注册配置预暂存的设备的唯一硬件标识。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 importedDeviceIdentities](../api/intune-enrollment-importeddeviceidentity-list.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) 集合|列出 [导入的DeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) 对象的属性和关系。|
|[获取 importedDeviceIdentity](../api/intune-enrollment-importeddeviceidentity-get.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|读取 [导入的DeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) 对象的属性和关系。|
|[创建 importedDeviceIdentity](../api/intune-enrollment-importeddeviceidentity-create.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|创建新的 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) 对象。|
|[删除 importedDeviceIdentity](../api/intune-enrollment-importeddeviceidentity-delete.md)|None|删除 [导入的DeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。|
|[更新 importedDeviceIdentity](../api/intune-enrollment-importeddeviceidentity-update.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|更新 [导入的DeviceIdentity 对象的](../resources/intune-enrollment-importeddeviceidentity.md) 属性。|
|[importDeviceIdentityList 操作](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) 集合|尚未记录|
|[searchExistingIdentities 操作](../api/intune-enrollment-importeddeviceidentity-searchexistingidentities.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) 集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|导入的设备标识的 ID|
|importedDeviceIdentifier|String|导入的设备标识符|
|importedDeviceIdentityType|[importedDeviceIdentityType](../resources/intune-enrollment-importeddeviceidentitytype.md)|导入的设备标识的类型。 可取值为：`unknown`、`imei`、`serialNumber`。|
|lastModifiedDateTime|DateTimeOffset|描述的最后一个修改日期时间|
|createdDateTime|DateTimeOffset|已创建设备的日期时间|
|lastContactedDateTime|DateTimeOffset|设备的上次联系日期时间|
|说明|String|设备的说明|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|Intune中的设备状态。 可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。|
|平台|[平台](../resources/intune-enrollment-platform.md)|设备的平台。 可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedDeviceIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "id": "String (identifier)",
  "importedDeviceIdentifier": "String",
  "importedDeviceIdentityType": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String"
}
```




