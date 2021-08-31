---
title: payloadCompatibleAssignmentFilter 资源类型
description: 一个包含用于有效负载兼容分配筛选器的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 260c0a90d458046c36603327ecd04a52947b288c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58793293"
---
# <a name="payloadcompatibleassignmentfilter-resource-type"></a>payloadCompatibleAssignmentFilter 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

一个包含用于有效负载兼容分配筛选器的属性的类。


继承自 [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 payloadCompatibleAssignmentFilters](../api/intune-policyset-payloadcompatibleassignmentfilter-list.md)|[payloadCompatibleAssignmentFilter](../resources/intune-policyset-payloadcompatibleassignmentfilter.md) 集合|列出 [payloadCompatibleAssignmentFilter](../resources/intune-policyset-payloadcompatibleassignmentfilter.md) 对象的属性和关系。|
|[获取 payloadCompatibleAssignmentFilter](../api/intune-policyset-payloadcompatibleassignmentfilter-get.md)|[payloadCompatibleAssignmentFilter](../resources/intune-policyset-payloadcompatibleassignmentfilter.md)|读取 [payloadCompatibleAssignmentFilter 对象的属性和](../resources/intune-policyset-payloadcompatibleassignmentfilter.md) 关系。|
|[创建 payloadCompatibleAssignmentFilter](../api/intune-policyset-payloadcompatibleassignmentfilter-create.md)|[payloadCompatibleAssignmentFilter](../resources/intune-policyset-payloadcompatibleassignmentfilter.md)|创建新的 [payloadCompatibleAssignmentFilter](../resources/intune-policyset-payloadcompatibleassignmentfilter.md) 对象。|
|[删除 payloadCompatibleAssignmentFilter](../api/intune-policyset-payloadcompatibleassignmentfilter-delete.md)|无|删除 [payloadCompatibleAssignmentFilter](../resources/intune-policyset-payloadcompatibleassignmentfilter.md)。|
|[更新 payloadCompatibleAssignmentFilter](../api/intune-policyset-payloadcompatibleassignmentfilter-update.md)|[payloadCompatibleAssignmentFilter](../resources/intune-policyset-payloadcompatibleassignmentfilter.md)|更新 [payloadCompatibleAssignmentFilter 对象](../resources/intune-policyset-payloadcompatibleassignmentfilter.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|工作分配筛选器的键。 继承自 [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|createdDateTime|DateTimeOffset|工作分配筛选器的创建时间。 继承自 [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|lastModifiedDateTime|DateTimeOffset|工作分配筛选器的上次修改时间。 继承自 [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|displayName|String|工作分配筛选器的 DisplayName。 继承自 [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|description|String|工作分配筛选器的说明。 继承自 [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|平台|[devicePlatformType](../resources/intune-policyset-deviceplatformtype.md)|工作分配筛选器适用的设备的平台类型。 继承自 [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)。 可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。|
|rule|String|工作分配筛选器的规则定义。 继承自 [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|roleScopeTags|String collection|工作分配筛选器的 RoleScopeTags。 继承自 [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|payloadType|[assignmentFilterPayloadType](../resources/intune-policyset-assignmentfilterpayloadtype.md)|工作分配筛选器的 PayloadType。 可取值为：`notSet`、`enrollmentRestrictions`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.payloadCompatibleAssignmentFilter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.payloadCompatibleAssignmentFilter",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "platform": "String",
  "rule": "String",
  "roleScopeTags": [
    "String"
  ],
  "payloadType": "String"
}
```



