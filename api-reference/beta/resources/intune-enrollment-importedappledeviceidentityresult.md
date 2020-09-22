---
title: importedAppleDeviceIdentityResult 资源类型
description: ImportedAppleDeviceIdentityResult 资源表示尝试导入 Apple 设备标识的结果。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 84cd09940d94c788f7cce1f2040cf392e8d0fb34
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080220"
---
# <a name="importedappledeviceidentityresult-resource-type"></a>importedAppleDeviceIdentityResult 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

ImportedAppleDeviceIdentityResult 资源表示尝试导入 Apple 设备标识的结果。


继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 importedAppleDeviceIdentityResults](../api/intune-enrollment-importedappledeviceidentityresult-list.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) 集合|列出 [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) 对象的属性和关系。|
|[获取 importedAppleDeviceIdentityResult](../api/intune-enrollment-importedappledeviceidentityresult-get.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)|读取 [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) 对象的属性和关系。|
|[创建 importedAppleDeviceIdentityResult](../api/intune-enrollment-importedappledeviceidentityresult-create.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)|创建新的 [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) 对象。|
|[删除 importedAppleDeviceIdentityResult](../api/intune-enrollment-importedappledeviceidentityresult-delete.md)|无|删除 [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)。|
|[更新 importedAppleDeviceIdentityResult](../api/intune-enrollment-importedappledeviceidentityresult-update.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)|更新 [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|serialNumber|String|继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)的设备序列号|
|requestedEnrollmentProfileId|String|注册配置文件 Id 管理员旨在在继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)的下一个注册过程中应用于设备|
|requestedEnrollmentProfileAssignmentDateTime|DateTimeOffset|将时间注册配置文件分配给继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)的设备|
|isSupervised|Boolean|指示 Apple 设备是否受到监督。 有关详细信息，请参阅 https://support.apple.com/HT202837 从[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)继承|
|discoverySource|[discoverySource](../resources/intune-enrollment-discoverysource.md)|Apple 设备发现源。 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。 可取值为：`unknown`、`adminImport`、`deviceEnrollmentProgram`。|
|isDeleted|Boolean|指示是否从[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)继承的 Apple Business Manager 中删除设备|
|createdDateTime|DateTimeOffset|从[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)继承的设备的创建日期时间|
|lastContactedDateTime|DateTimeOffset|从[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)继承的设备的上次联系日期时间|
|说明|String|从[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)继承的设备的说明|
|enrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|Intune 中的设备的状态继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。 可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。|
|平台|[平台](../resources/intune-enrollment-platform.md)|设备的平台。 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。 可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。|
|状态|Boolean|导入的设备标识的状态|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedAppleDeviceIdentityResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
  "id": "String (identifier)",
  "serialNumber": "String",
  "requestedEnrollmentProfileId": "String",
  "requestedEnrollmentProfileAssignmentDateTime": "String (timestamp)",
  "isSupervised": true,
  "discoverySource": "String",
  "isDeleted": true,
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String",
  "status": true
}
```






