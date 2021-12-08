---
title: hardwareConfigurationRunSummary 资源类型
description: 包含硬件配置脚本的运行摘要的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6debf44d50ff1f501af172de706165c22dd02642
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61345418"
---
# <a name="hardwareconfigurationrunsummary-resource-type"></a>hardwareConfigurationRunSummary 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含硬件配置脚本的运行摘要的属性。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 hardwareConfigurationRunSummary](../api/intune-deviceconfig-hardwareconfigurationrunsummary-get.md)|[hardwareConfigurationRunSummary](../resources/intune-deviceconfig-hardwareconfigurationrunsummary.md)|读取 [hardwareConfigurationRunSummary 对象的属性和](../resources/intune-deviceconfig-hardwareconfigurationrunsummary.md) 关系。|
|[更新 hardwareConfigurationRunSummary](../api/intune-deviceconfig-hardwareconfigurationrunsummary-update.md)|[hardwareConfigurationRunSummary](../resources/intune-deviceconfig-hardwareconfigurationrunsummary.md)|更新 [hardwareConfigurationRunSummary 对象](../resources/intune-deviceconfig-hardwareconfigurationrunsummary.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|硬件配置运行摘要实体的键。 此属性是只读的。|
|successfulDeviceCount|Int32|已配置硬件而未出现任何问题的设备数量|
|failedDeviceCount|Int32|硬件配置发现问题的设备数量|
|pendingDeviceCount|Int32|其硬件配置为待定状态的设备数量|
|errorDeviceCount|Int32|硬件配置状态为错误的设备数量|
|notApplicableDeviceCount|Int32|硬件配置状态不适用的设备数量|
|unknownDeviceCount|Int32|硬件配置状态未知的设备数量|
|successfulUserCount|Int32|未出现任何问题的情况下配置其硬件的用户数量|
|failedUserCount|Int32|硬件配置发现问题的用户数量|
|pendingUserCount|Int32|其硬件配置为待定状态的用户数量|
|errorUserCount|Int32|硬件配置状态为错误的用户数量|
|notApplicableUserCount|Int32|硬件配置状态不适用的用户数量|
|unknownUserCount|Int32|硬件配置状态未知用户的数量|
|lastRunDateTime|DateTimeOffset|跨所有设备的配置的上次运行时间|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.hardwareConfigurationRunSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hardwareConfigurationRunSummary",
  "id": "String (identifier)",
  "successfulDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "pendingDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "successfulUserCount": 1024,
  "failedUserCount": 1024,
  "pendingUserCount": 1024,
  "errorUserCount": 1024,
  "notApplicableUserCount": 1024,
  "unknownUserCount": 1024,
  "lastRunDateTime": "String (timestamp)"
}
```




