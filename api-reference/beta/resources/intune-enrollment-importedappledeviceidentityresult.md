---
title: importedAppleDeviceIdentityResult 资源类型
description: importedAppleDeviceIdentityResult 资源表示尝试导入 Apple 设备标识的结果。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 22e21105a508d613aeaeb73fb4547d5f800d7a44
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033509"
---
# <a name="importedappledeviceidentityresult-resource-type"></a>importedAppleDeviceIdentityResult 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

importedAppleDeviceIdentityResult 资源表示尝试导入 Apple 设备标识的结果。


继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 importedAppleDeviceIdentityResults](../api/intune-enrollment-importedappledeviceidentityresult-list.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) 集合|列出 [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) 对象的属性和关系。|
|[获取 importedAppleDeviceIdentityResult](../api/intune-enrollment-importedappledeviceidentityresult-get.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)|读取 [importedAppleDeviceIdentityResult 对象的属性和](../resources/intune-enrollment-importedappledeviceidentityresult.md) 关系。|
|[创建 importedAppleDeviceIdentityResult](../api/intune-enrollment-importedappledeviceidentityresult-create.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)|创建新的 [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) 对象。|
|[删除 importedAppleDeviceIdentityResult](../api/intune-enrollment-importedappledeviceidentityresult-delete.md)|无|删除 [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)。|
|[更新 importedAppleDeviceIdentityResult](../api/intune-enrollment-importedappledeviceidentityresult-update.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)|更新 [importedAppleDeviceIdentityResult 对象](../resources/intune-enrollment-importedappledeviceidentityresult.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|serialNumber|String|设备序列号 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|requestedEnrollmentProfileId|String|注册配置文件 ID 管理员打算在下一次注册期间应用到设备 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|requestedEnrollmentProfileAssignmentDateTime|DateTimeOffset|向设备分配注册配置文件的时间 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|isSupervised|Boolean|指示 Apple 设备是否受监督。 详细信息位于： https://support.apple.com/en-us/HT202837 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|discoverySource|[discoverySource](../resources/intune-enrollment-discoverysource.md)|Apple 设备发现源。 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。 可取值为：`unknown`、`adminImport`、`deviceEnrollmentProgram`。|
|isDeleted|Boolean|指示设备是否从 Apple Business Manager 中删除 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|createdDateTime|DateTimeOffset|设备的创建日期时间 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|lastContactedDateTime|DateTimeOffset|设备的上次联系日期时间 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|说明|String|设备描述 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|enrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|Intune 中的设备状态 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。 可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。|
|平台|[平台](../resources/intune-enrollment-platform.md)|设备平台。 继承自 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。 可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。|
|status|Boolean|导入的设备标识的状态|

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



