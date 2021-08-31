---
title: importedDeviceIdentityResult 资源类型
description: importedDeviceIdentityResult 资源表示尝试导入设备标识的结果。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ce45e2556fde4632227afe16ff270de2ec68c471
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58785729"
---
# <a name="importeddeviceidentityresult-resource-type"></a>importedDeviceIdentityResult 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

importedDeviceIdentityResult 资源表示尝试导入设备标识的结果。


继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 importedDeviceIdentityResults](../api/intune-enrollment-importeddeviceidentityresult-list.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) 集合|列出 [importedDeviceIdentityResult 对象的属性和](../resources/intune-enrollment-importeddeviceidentityresult.md) 关系。|
|[获取 importedDeviceIdentityResult](../api/intune-enrollment-importeddeviceidentityresult-get.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|读取 [importedDeviceIdentityResult 对象的属性和](../resources/intune-enrollment-importeddeviceidentityresult.md) 关系。|
|[创建 importedDeviceIdentityResult](../api/intune-enrollment-importeddeviceidentityresult-create.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|创建新的 [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) 对象。|
|[删除 importedDeviceIdentityResult](../api/intune-enrollment-importeddeviceidentityresult-delete.md)|无|删除 [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)。|
|[更新 importedDeviceIdentityResult](../api/intune-enrollment-importeddeviceidentityresult-update.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|更新 [importedDeviceIdentityResult 对象](../resources/intune-enrollment-importeddeviceidentityresult.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|导入的设备标识的 ID 继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|importedDeviceIdentifier|String|导入的设备标识符 继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|importedDeviceIdentityType|[importedDeviceIdentityType](../resources/intune-enrollment-importeddeviceidentitytype.md)|导入的设备标识的类型 继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。 可取值为：`unknown`、`imei`、`serialNumber`。|
|lastModifiedDateTime|DateTimeOffset|说明的 Last Modified DateTime 继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|createdDateTime|DateTimeOffset|设备的创建日期时间 继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|lastContactedDateTime|DateTimeOffset|设备的上次联系日期时间 继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|description|String|设备描述 继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|enrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|Intune 中的设备状态 继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。 可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。|
|平台|[平台](../resources/intune-enrollment-platform.md)|设备平台。 继承自 [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)。 可取值为：`unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。|
|状态|Boolean|导入的设备标识的状态|

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



