---
title: hardwareConfigurationUserState 资源类型
description: 包含硬件配置的用户状态的属性
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3a9fab2a1b312e9b18ff38f5548e964a5256335f
ms.sourcegitcommit: 00ac72f7b1cdde4f71ff332c2e7953908ef9de52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/04/2022
ms.locfileid: "61711975"
---
# <a name="hardwareconfigurationuserstate-resource-type"></a>hardwareConfigurationUserState 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含硬件配置的用户状态的属性

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 hardwareConfigurationUserStates](../api/intune-deviceconfig-hardwareconfigurationuserstate-list.md)|[hardwareConfigurationUserState](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md) 集合|列出 [hardwareConfigurationUserState 对象的属性和](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md) 关系。|
|[获取 hardwareConfigurationUserState](../api/intune-deviceconfig-hardwareconfigurationuserstate-get.md)|[hardwareConfigurationUserState](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md)|读取 [hardwareConfigurationUserState 对象的属性和](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md) 关系。|
|[创建 hardwareConfigurationUserState](../api/intune-deviceconfig-hardwareconfigurationuserstate-create.md)|[hardwareConfigurationUserState](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md)|创建新的 [hardwareConfigurationUserState](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md) 对象。|
|[删除 hardwareConfigurationUserState](../api/intune-deviceconfig-hardwareconfigurationuserstate-delete.md)|None|删除 [hardwareConfigurationUserState](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md)。|
|[更新 hardwareConfigurationUserState](../api/intune-deviceconfig-hardwareconfigurationuserstate-update.md)|[hardwareConfigurationUserState](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md)|更新 [hardwareConfigurationUserState 对象](../resources/intune-deviceconfig-hardwareconfigurationuserstate.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|硬件配置脚本用户状态实体的键。 此属性是只读的。|
|upn|String|用户主体名称 (UPN)。|
|userEmail|String|用户电子邮件地址。|
|userName|String|用户名|
|lastStateUpdateDateTime|DateTimeOffset|上次执行硬件配置的时间戳|
|successfulDeviceCount|Int32|特定用户的成功设备计数。|
|failedDeviceCount|Int32|特定用户的设备计数失败。|
|pendingDeviceCount|Int32|特定用户的挂起设备计数。|
|errorDeviceCount|Int32|特定用户的错误设备计数。|
|notApplicableDeviceCount|Int32|不适用于特定用户的设备计数。|
|unknownDeviceCount|Int32|特定用户的未知设备计数。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.hardwareConfigurationUserState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hardwareConfigurationUserState",
  "id": "String (identifier)",
  "upn": "String",
  "userEmail": "String",
  "userName": "String",
  "lastStateUpdateDateTime": "String (timestamp)",
  "successfulDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "pendingDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "unknownDeviceCount": 1024
}
```




