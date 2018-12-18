---
title: importedAppleDeviceIdentityResult 资源类型
description: ImportedAppleDeviceIdentityResult 资源表示尝试导入 Apple 设备标识的结果。
author: tfitzmac
ms.openlocfilehash: 650dfca3cba7800c2cdc9eb0087e9d67b8dc0b29
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344560"
---
# <a name="importedappledeviceidentityresult-resource-type"></a>importedAppleDeviceIdentityResult 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

ImportedAppleDeviceIdentityResult 资源表示尝试导入 Apple 设备标识的结果。

继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 importedAppleDeviceIdentityResults](../api/intune-enrollment-importedappledeviceidentityresult-list.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)集合|列出属性和[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)对象之间的关系。|
|[获取 importedAppleDeviceIdentityResult](../api/intune-enrollment-importedappledeviceidentityresult-get.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)|读取属性和[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)对象的关系。|
|[创建 importedAppleDeviceIdentityResult](../api/intune-enrollment-importedappledeviceidentityresult-create.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)|创建新的[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)对象。|
|[删除 importedAppleDeviceIdentityResult](../api/intune-enrollment-importedappledeviceidentityresult-delete.md)|无|删除[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)。|
|[更新 importedAppleDeviceIdentityResult](../api/intune-enrollment-importedappledeviceidentityresult-update.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)|更新[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|serialNumber|字符串|从[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)设备序列号继承|
|requestedEnrollmentProfileId|字符串|注册配置文件 Id 管理打算在下一步注册继承过程中从[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)适用于设备|
|requestedEnrollmentProfileAssignmentDateTime|DateTimeOffset|从[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)时间注册配置文件分配给设备继承|
|isSupervised|Boolean|指示是否管理 Apple 设备。 详细信息位于：https://support.apple.com/en-us/HT202837继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|discoverySource|[discoverySource](../resources/intune-enrollment-discoverysource.md)|Apple 设备发现源。 继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。 可取值为：`unknown`、`adminImport`、`deviceEnrollmentProgram`。|
|createdDateTime|DateTimeOffset|从[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)创建设备继承的日期时间|
|lastContactedDateTime|DateTimeOffset|从[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)设备继承的最后一个联系日期时间|
|说明|字符串|从[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)设备继承说明|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|从[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)中 Intune 继承的设备的状态。 可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。|
|platform|[平台](../resources/intune-enrollment-platform.md)|设备的平台。 继承自[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)。 可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。|
|status|Boolean|导入的设备标识的状态|

## <a name="relationships"></a>Relationships
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
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String",
  "status": true
}
```





