---
title: windowsInformationProtectionWipeAction 资源类型
description: 表示租户管理员针对自带设备办公和 BYOD 设备 (擦除) Windows请求。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: aac1b49d6c2fab449fda91bdb5a339099950530e
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58786942"
---
# <a name="windowsinformationprotectionwipeaction-resource-type"></a>windowsInformationProtectionWipeAction 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示租户管理员针对自带设备办公和 BYOD 设备 (擦除) Windows请求。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsInformationProtectionWipeActions](../api/intune-mam-windowsinformationprotectionwipeaction-list.md)|[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) 集合|列出 [windowsInformationProtectionWipeAction 对象的属性和](../resources/intune-mam-windowsinformationprotectionwipeaction.md) 关系。|
|[获取 windowsInformationProtectionWipeAction](../api/intune-mam-windowsinformationprotectionwipeaction-get.md)|[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|读取 [windowsInformationProtectionWipeAction 对象的属性和](../resources/intune-mam-windowsinformationprotectionwipeaction.md) 关系。|
|[创建 windowsInformationProtectionWipeAction](../api/intune-mam-windowsinformationprotectionwipeaction-create.md)|[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|创建新的 [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) 对象。|
|[删除 windowsInformationProtectionWipeAction](../api/intune-mam-windowsinformationprotectionwipeaction-delete.md)|无|删除 [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)。|
|[更新 windowsInformationProtectionWipeAction](../api/intune-mam-windowsinformationprotectionwipeaction-update.md)|[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|更新 [windowsInformationProtectionWipeAction 对象](../resources/intune-mam-windowsinformationprotectionwipeaction.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|状态|[actionState](../resources/intune-shared-actionstate.md)|擦除操作状态。 可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。|
|targetedUserId|String|此擦除操作所针对的 UserId。|
|targetedDeviceRegistrationId|字符串|此擦除操作所针对的 DeviceRegistrationId。|
|targetedDeviceName|字符串|目标设备名称。|
|targetedDeviceMacAddress|String|目标设备 Mac 地址。|
|lastCheckInDateTime|DateTimeOffset|此擦除操作针对的设备的最后签入时间。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionWipeAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "id": "String (identifier)",
  "status": "String",
  "targetedUserId": "String",
  "targetedDeviceRegistrationId": "String",
  "targetedDeviceName": "String",
  "targetedDeviceMacAddress": "String",
  "lastCheckInDateTime": "String (timestamp)"
}
```



