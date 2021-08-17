---
title: deviceAndAppManagementAssignmentFilter 资源类型
description: 一个包含用于工作分配筛选器的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 135594e3dd1ea54b6ca61b0724a31537519258c9
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266826"
---
# <a name="deviceandappmanagementassignmentfilter-resource-type"></a>deviceAndAppManagementAssignmentFilter 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

一个包含用于工作分配筛选器的属性的类。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceAndAppManagementAssignmentFilters](../api/intune-policyset-deviceandappmanagementassignmentfilter-list.md)|[deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) 集合|列出 [deviceAndAppManagementAssignmentFilter 对象的属性和](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) 关系。|
|[获取 deviceAndAppManagementAssignmentFilter](../api/intune-policyset-deviceandappmanagementassignmentfilter-get.md)|[deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|读取 [deviceAndAppManagementAssignmentFilter 对象的属性和](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) 关系。|
|[创建 deviceAndAppManagementAssignmentFilter](../api/intune-policyset-deviceandappmanagementassignmentfilter-create.md)|[deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|创建新的 [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) 对象。|
|[删除 deviceAndAppManagementAssignmentFilter](../api/intune-policyset-deviceandappmanagementassignmentfilter-delete.md)|无|删除 [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)。|
|[更新 deviceAndAppManagementAssignmentFilter](../api/intune-policyset-deviceandappmanagementassignmentfilter-update.md)|[deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|更新 [deviceAndAppManagementAssignmentFilter 对象](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) 的属性。|
|[validateFilter 操作](../api/intune-policyset-deviceandappmanagementassignmentfilter-validatefilter.md)|[assignmentFilterValidationResult](../resources/intune-policyset-assignmentfiltervalidationresult.md)|尚未记录|
|[启用操作](../api/intune-policyset-deviceandappmanagementassignmentfilter-enable.md)|无|尚未记录|
|[getState 函数](../api/intune-policyset-deviceandappmanagementassignmentfilter-getstate.md)|[assignmentFilterState](../resources/intune-policyset-assignmentfilterstate.md)|尚未记录|
|[getPlatformSupportedProperties 函数](../api/intune-policyset-deviceandappmanagementassignmentfilter-getplatformsupportedproperties.md)|[assignmentFilterSupportedProperty](../resources/intune-policyset-assignmentfiltersupportedproperty.md) 集合|尚未记录|
|[getSupportedProperties 函数](../api/intune-policyset-deviceandappmanagementassignmentfilter-getsupportedproperties.md)|[assignmentFilterSupportedProperty](../resources/intune-policyset-assignmentfiltersupportedproperty.md) 集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|工作分配筛选器的键。|
|createdDateTime|DateTimeOffset|工作分配筛选器的创建时间。|
|lastModifiedDateTime|DateTimeOffset|工作分配筛选器的上次修改时间。|
|displayName|字符串|工作分配筛选器的 DisplayName。|
|description|String|工作分配筛选器的说明。|
|平台|[devicePlatformType](../resources/intune-policyset-deviceplatformtype.md)|工作分配筛选器适用的设备的平台类型。 可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。|
|rule|字符串|工作分配筛选器的规则定义。|
|roleScopeTags|String collection|工作分配筛选器的 RoleScopeTags。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentFilter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignmentFilter",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "platform": "String",
  "rule": "String",
  "roleScopeTags": [
    "String"
  ]
}
```




