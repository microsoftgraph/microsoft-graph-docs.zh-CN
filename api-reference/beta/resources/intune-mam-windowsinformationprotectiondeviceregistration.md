---
title: windowsInformationProtectionDeviceRegistration 资源类型
description: 代表 Bring-Your-Own-Device (BYOD) Windows记录。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 68c8ed0f9c4b214d95d286db00a4732587ce188fa548219181048b4ea13705c3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54248271"
---
# <a name="windowsinformationprotectiondeviceregistration-resource-type"></a>windowsInformationProtectionDeviceRegistration 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

代表 Bring-Your-Own-Device (BYOD) Windows记录。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsInformationProtectionDeviceRegistrations](../api/intune-mam-windowsinformationprotectiondeviceregistration-list.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) 集合|列出 [windowsInformationProtectionDeviceRegistration 对象的属性和](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) 关系。|
|[获取 windowsInformationProtectionDeviceRegistration](../api/intune-mam-windowsinformationprotectiondeviceregistration-get.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|读取 [windowsInformationProtectionDeviceRegistration 对象的属性和](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) 关系。|
|[创建 windowsInformationProtectionDeviceRegistration](../api/intune-mam-windowsinformationprotectiondeviceregistration-create.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|创建新的 [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) 对象。|
|[删除 windowsInformationProtectionDeviceRegistration](../api/intune-mam-windowsinformationprotectiondeviceregistration-delete.md)|无|删除 [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)。|
|[更新 windowsInformationProtectionDeviceRegistration](../api/intune-mam-windowsinformationprotectiondeviceregistration-update.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|更新 [windowsInformationProtectionDeviceRegistration 对象](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) 的属性。|
|[wipe 操作](../api/intune-mam-windowsinformationprotectiondeviceregistration-wipe.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|userId|字符串|与此设备注册记录关联的 UserId。|
|deviceRegistrationId|字符串|此设备注册记录的设备标识符。|
|deviceName|String|设备名称。|
|deviceType|String|设备类型，例如，Windows笔记本电脑 VS Windows电话。|
|deviceMacAddress|String|设备 Mac 地址。|
|lastCheckInDateTime|DateTimeOffset|设备的上次签入时间。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDeviceRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDeviceRegistration",
  "id": "String (identifier)",
  "userId": "String",
  "deviceRegistrationId": "String",
  "deviceName": "String",
  "deviceType": "String",
  "deviceMacAddress": "String",
  "lastCheckInDateTime": "String (timestamp)"
}
```




