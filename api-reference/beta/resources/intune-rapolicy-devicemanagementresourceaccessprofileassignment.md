---
title: deviceManagementResourceAccessProfileAssignment 资源类型
description: 描述派生凭据的租户级别设置的实体
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 608e63b6b41ef6cc8f6a0f9b45d3aec2d00316a6
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58806584"
---
# <a name="devicemanagementresourceaccessprofileassignment-resource-type"></a>deviceManagementResourceAccessProfileAssignment 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

描述派生凭据的租户级别设置的实体

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementResourceAccessProfileAssignments](../api/intune-rapolicy-devicemanagementresourceaccessprofileassignment-list.md)|[deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) 集合|列出 [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) 对象的属性和关系。|
|[获取 deviceManagementResourceAccessProfileAssignment](../api/intune-rapolicy-devicemanagementresourceaccessprofileassignment-get.md)|[deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|读取 [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) 对象的属性和关系。|
|[创建 deviceManagementResourceAccessProfileAssignment](../api/intune-rapolicy-devicemanagementresourceaccessprofileassignment-create.md)|[deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|创建新的 [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) 对象。|
|[删除 deviceManagementResourceAccessProfileAssignment](../api/intune-rapolicy-devicemanagementresourceaccessprofileassignment-delete.md)|无|删除 [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)。|
|[更新 deviceManagementResourceAccessProfileAssignment](../api/intune-rapolicy-devicemanagementresourceaccessprofileassignment-update.md)|[deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|更新 [deviceManagementResourceAccessProfileAssignment 对象](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|工作分配的唯一标识符|
|intent|[deviceManagementResourceAccessProfileIntent](../resources/intune-rapolicy-devicemanagementresourceaccessprofileintent.md)|资源访问配置文件的分配意图。 可取值为：`apply`、`remove`。|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|资源访问配置文件的分配目标。|
|sourceId|String|工作分配的源的标识符。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementResourceAccessProfileAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementResourceAccessProfileAssignment",
  "id": "String (identifier)",
  "intent": "String",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  },
  "sourceId": "String"
}
```



