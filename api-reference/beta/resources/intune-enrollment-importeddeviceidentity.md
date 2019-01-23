---
title: importedDeviceIdentity 资源类型
description: ImportedDeviceIdentity 资源表示预注册配置已预暂存设备的唯一的硬件标识。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c151257a95d1161e07de17ed6d9fc01fc021146e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421443"
---
# <a name="importeddeviceidentity-resource-type"></a>importedDeviceIdentity 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

ImportedDeviceIdentity 资源表示预注册配置已预暂存设备的唯一的硬件标识。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 importedDeviceIdentities](../api/intune-enrollment-importeddeviceidentity-list.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)集合|列出属性和[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象之间的关系。|
|[获取 importedDeviceIdentity](../api/intune-enrollment-importeddeviceidentity-get.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|读取属性和[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象的关系。|
|[创建 importedDeviceIdentity](../api/intune-enrollment-importeddeviceidentity-create.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|创建新的[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象。|
|[删除 importedDeviceIdentity](../api/intune-enrollment-importeddeviceidentity-delete.md)|无|删除[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。|
|[更新 importedDeviceIdentity](../api/intune-enrollment-importeddeviceidentity-update.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|更新[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象的属性。|
|[importDeviceIdentityList 操作](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|导入的设备标识的 id|
|importedDeviceIdentifier|String|导入的设备标识符|
|importedDeviceIdentityType|[importedDeviceIdentityType](../resources/intune-enrollment-importeddeviceidentitytype.md)|导入的设备的标识的类型。 可取值为：`unknown`、`imei`、`serialNumber`。|
|lastModifiedDateTime|DateTimeOffset|上次修改日期时间的说明|
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




