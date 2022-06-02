---
title: userExperienceAnalyticsDeviceScope 资源类型
description: 用户体验分析设备范围实体包含用于在终结点分析报表上应用筛选的设备范围配置值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cf5605a0f65dcf4e4d35026bf18d5499ab2a6c96
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858556"
---
# <a name="userexperienceanalyticsdevicescope-resource-type"></a>userExperienceAnalyticsDeviceScope 资源类型

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析设备范围实体包含用于在终结点分析报表上应用筛选的设备范围配置值。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsDeviceScopes](../api/intune-devices-userexperienceanalyticsdevicescope-list.md)|[userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md) 集合|列出 [userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md) 对象的属性和关系。|
|[获取 userExperienceAnalyticsDeviceScope](../api/intune-devices-userexperienceanalyticsdevicescope-get.md)|[userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md)|读取 [userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md) 对象的属性和关系。|
|[创建 userExperienceAnalyticsDeviceScope](../api/intune-devices-userexperienceanalyticsdevicescope-create.md)|[userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md)|创建新的 [userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md) 对象。|
|[删除 userExperienceAnalyticsDeviceScope](../api/intune-devices-userexperienceanalyticsdevicescope-delete.md)|None|删除 [userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md)。|
|[更新 userExperienceAnalyticsDeviceScope](../api/intune-devices-userexperienceanalyticsdevicescope-update.md)|[userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md)|更新 [userExperienceAnalyticsDeviceScope](../resources/intune-devices-userexperienceanalyticsdevicescope.md) 对象的属性。|
|[triggerDeviceScopeAction 操作](../api/intune-devices-userexperienceanalyticsdevicescope-triggerdevicescopeaction.md)|[deviceScopeActionResult](../resources/intune-devices-devicescopeactionresult.md)|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设备范围配置的唯一标识符。|
|deviceScopeName|String|用户体验分析设备范围配置的名称。|
|ownerId|String|创建设备范围配置的管理员)  (人员的唯一标识符。|
|isBuiltIn|Boolean|指示设备范围配置是内置配置还是自定义配置。 如果为 TRUE，则设备范围配置是内置的。 如果为 FALSE，则设备范围配置为自定义。 默认值为 FALSE。|
|enabled|Boolean|指示设备范围是已启用还是已禁用。 如果为 TRUE，则启用设备范围。 如果为 FALSE，则禁用设备范围。 默认值为 FALSE。|
|status|[deviceScopeStatus](../resources/intune-devices-devicescopestatus.md)|指示设备范围启用后的设备范围状态。 可能的值为：none、computing、insufficientData 或 completed。 默认值为无。 可取值为：`none`、`computing`、`insufficientData`、`completed`、`unknownFutureValue`。|
|形参|[deviceScopeParameter](../resources/intune-devices-devicescopeparameter.md)|设备范围配置参数。 将来将扩展它以添加更多参数。 Eg：设备范围参数可以是 OS 版本、磁盘类型、设备制造商、设备模型或范围标记。 默认值：scopeTag。 可取值为：`none`、`scopeTag`、`unknownFutureValue`。|
|operator|[deviceScopeOperator](../resources/intune-devices-devicescopeoperator.md)|设备范围配置查询运算符。 可能的值为：equals、notEquals、contains、notContains、greaterThan、lessThan。 默认值：等于。 可取值为：`none`、`equals`、`unknownFutureValue`。|
|valueObjectId|String|用于创建设备范围配置的用户设备范围标记 ID 的唯一标识符。|
|value|String|设备范围配置查询子句值。|
|createdDateTime|DateTimeOffset|指示自定义设备范围的创建日期和时间。|
|lastModifiedDateTime|DateTimeOffset|指示自定义设备范围的上次更新日期和时间。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsDeviceScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceScope",
  "id": "String (identifier)",
  "deviceScopeName": "String",
  "ownerId": "String",
  "isBuiltIn": true,
  "enabled": true,
  "status": "String",
  "parameter": "String",
  "operator": "String",
  "valueObjectId": "String",
  "value": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




