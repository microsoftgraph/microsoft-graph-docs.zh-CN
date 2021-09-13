---
title: importedAppleDeviceIdentity 资源类型
description: importedAppleDeviceIdentity 资源表示 Apple 设备的导入设备标识。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f0e66ebabdfd4466d187778313644c83e5dfb542
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59141072"
---
# <a name="importedappledeviceidentity-resource-type"></a>importedAppleDeviceIdentity 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

importedAppleDeviceIdentity 资源表示 Apple 设备的导入设备标识。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 importedAppleDeviceIdentities](../api/intune-enrollment-importedappledeviceidentity-list.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) 集合|列出 [importedAppleDeviceIdentity 对象的属性和](../resources/intune-enrollment-importedappledeviceidentity.md) 关系。|
|[获取 importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-get.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|读取 [importedAppleDeviceIdentity 对象的属性和](../resources/intune-enrollment-importedappledeviceidentity.md) 关系。|
|[创建 importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-create.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|创建新的 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) 对象。|
|[删除 importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-delete.md)|无|删除 [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。|
|[更新 importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-update.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|更新 [importedAppleDeviceIdentity 对象](../resources/intune-enrollment-importedappledeviceidentity.md) 的属性。|
|[importAppleDeviceIdentityList 操作](../api/intune-enrollment-importedappledeviceidentity-importappledeviceidentitylist.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) 集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|serialNumber|String|设备序列号|
|requestedEnrollmentProfileId|String|注册配置文件 ID 管理员打算在下一次注册期间应用到设备|
|requestedEnrollmentProfileAssignmentDateTime|DateTimeOffset|向设备分配注册配置文件的时间|
|isSupervised|Boolean|指示 Apple 设备是否受监督。 有关详细信息，请参阅： https://support.apple.com/en-us/HT202837|
|discoverySource|[discoverySource](../resources/intune-enrollment-discoverysource.md)|Apple 设备发现源。 可取值为：`unknown`、`adminImport`、`deviceEnrollmentProgram`。|
|isDeleted|Boolean|指示设备是否从 Apple Business Manager 中删除|
|createdDateTime|DateTimeOffset|设备的创建日期时间|
|lastContactedDateTime|DateTimeOffset|设备的上次联系日期时间|
|说明|String|设备说明|
|enrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|Intune 中的设备状态。 可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。|
|平台|[平台](../resources/intune-enrollment-platform.md)|设备平台。 可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。|

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
  "isDeleted": true,
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String"
}
```



