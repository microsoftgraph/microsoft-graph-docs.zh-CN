---
title: importedAppleDeviceIdentity 资源类型
description: ImportedAppleDeviceIdentity 资源表示 Apple 设备的导入的设备标识。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ae0f940614ae8b872891579957e8f86c92342da8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416823"
---
# <a name="importedappledeviceidentity-resource-type"></a>importedAppleDeviceIdentity 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

ImportedAppleDeviceIdentity 资源表示 Apple 设备的导入的设备标识。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 importedAppleDeviceIdentities](../api/intune-enrollment-importedappledeviceidentity-list.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)集合|列出属性和[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象之间的关系。|
|[获取 importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-get.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|读取属性和[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象的关系。|
|[创建 importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-create.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|创建新的[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象。|
|[删除 importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-delete.md)|无|删除[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。|
|[更新 importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-update.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|更新[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)对象的属性。|
|[importAppleDeviceIdentityList 操作](../api/intune-enrollment-importedappledeviceidentity-importappledeviceidentitylist.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|serialNumber|String|设备序列号|
|requestedEnrollmentProfileId|String|注册配置文件 Id 管理打算在下一步注册过程适用于设备|
|requestedEnrollmentProfileAssignmentDateTime|DateTimeOffset|时间注册配置文件分配给设备|
|isSupervised|Boolean|指示是否管理 Apple 设备。 详细信息位于：https://support.apple.com/en-us/HT202837|
|discoverySource|[discoverySource](../resources/intune-enrollment-discoverysource.md)|Apple 设备发现源。 可取值为：`unknown`、`adminImport`、`deviceEnrollmentProgram`。|
|createdDateTime|DateTimeOffset|设备的创建的日期时间|
|lastContactedDateTime|DateTimeOffset|设备的最后一个联系日期时间|
|说明|String|设备的说明|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|在 Intune 设备的状态。 可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。|
|platform|[平台](../resources/intune-enrollment-platform.md)|设备的平台。 可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedAppleDeviceIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "id": "String (identifier)",
  "serialNumber": "String",
  "requestedEnrollmentProfileId": "String",
  "requestedEnrollmentProfileAssignmentDateTime": "String (timestamp)",
  "isSupervised": true,
  "discoverySource": "String",
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String"
}
```




