---
title: circularGeofenceManagementCondition 资源类型
description: 包含用于定义要监视的循环地理围栏管理条件（一个关注区域）的信息。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 32032ef83f3a724ecc98fd1134d40d95b1a76dcf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59030296"
---
# <a name="circulargeofencemanagementcondition-resource-type"></a>circularGeofenceManagementCondition 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于定义要监视的循环地理围栏管理条件（一个关注区域）的信息。


继承自 [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 circularGeofenceManagementConditions](../api/intune-fencing-circulargeofencemanagementcondition-list.md)|[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) 集合|列出 [circularGeofenceManagementCondition 对象的属性和](../resources/intune-fencing-circulargeofencemanagementcondition.md) 关系。|
|[获取 circularGeofenceManagementCondition](../api/intune-fencing-circulargeofencemanagementcondition-get.md)|[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)|读取 [circularGeofenceManagementCondition 对象的属性和](../resources/intune-fencing-circulargeofencemanagementcondition.md) 关系。|
|[创建 circularGeofenceManagementCondition](../api/intune-fencing-circulargeofencemanagementcondition-create.md)|[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)|创建新的 [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) 对象。|
|[删除 circularGeofenceManagementCondition](../api/intune-fencing-circulargeofencemanagementcondition-delete.md)|无|删除 [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)。|
|[更新 circularGeofenceManagementCondition](../api/intune-fencing-circulargeofencemanagementcondition-update.md)|[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)|更新 [circularGeofenceManagementCondition 对象](../resources/intune-fencing-circulargeofencemanagementcondition.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|管理条件的唯一标识符。 创建时分配的系统生成值。 继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)|
|唯一名称|String|管理条件的唯一名称。 在管理条件表达式中使用。 继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)|
|displayName|String|管理员定义的管理条件名称。 继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)|
|说明|String|管理员定义的管理条件说明。 继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|创建管理条件的时间。 生成的服务器端。 继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|上次修改管理条件的时间。 更新的服务器端。 继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)|
|eTag|String|管理条件的 ETag。 更新的服务器端。 继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)|
|applicablePlatforms|[devicePlatformType](../resources/intune-fencing-deviceplatformtype.md) 集合|此管理条件的适用平台。 继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)|
|latitude|Double|纬度（以度数表示），介于 -90 和 +90 之间（含这两者）。|
|longitude|Double|以度数表示的经度，介于 -180 和 +180 之间（含这两者）。|
|radiusInMeters|单一|以米为单位的半径。|

## <a name="relationships"></a>关系
|关系|类型|描述|
|:---|:---|:---|
|managementConditionStatements|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) 集合|与管理条件关联的管理条件语句。 继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.circularGeofenceManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.circularGeofenceManagementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ],
  "latitude": "4.2",
  "longitude": "4.2",
  "radiusInMeters": 4.2
}
```



