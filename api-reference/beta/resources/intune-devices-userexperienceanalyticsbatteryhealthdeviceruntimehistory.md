---
title: userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory 资源类型
description: 用户体验分析电池运行状况运行时历史记录实体包含 30 天内设备的运行时趋势
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 46c88e9bccacade261ca1dbe8f10e43a3e9b4d68
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61338769"
---
# <a name="userexperienceanalyticsbatteryhealthdeviceruntimehistory-resource-type"></a>userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析电池运行状况运行时历史记录实体包含 30 天内设备的运行时趋势

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsBatteryHealthDeviceRuntimeHistories](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory-list.md)|[userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md) 集合|列出 [userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory 对象的属性和](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md) 关系。|
|[获取 userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory-get.md)|[userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md)|读取 [userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory 对象的属性和](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md) 关系。|
|[创建 userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory-create.md)|[userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md)|创建新的 [userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md) 对象。|
|[删除 userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory-delete.md)|无|删除 [userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md)。|
|[更新 userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory-update.md)|[userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md)|更新 [userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory 对象](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析电池运行状况运行时对象的唯一标识符。|
|deviceId|String|设备的唯一标识符，Intune DeviceID 或 SCCM 设备 ID。|
|runtimeDateTime|String|运行时历史记录实例的日期时间。|
|estimatedRuntimeInMinutes|Int32|电池完全充电时设备的预计运行时。 单位（以分钟表示）。 有效值 -2147483648 to 2147483647|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory",
  "id": "String (identifier)",
  "deviceId": "String",
  "runtimeDateTime": "String",
  "estimatedRuntimeInMinutes": 1024
}
```




