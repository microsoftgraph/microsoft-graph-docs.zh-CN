---
title: managedEBookAssignment 资源类型
description: 包含用于为组分配电子书的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 35efc1e9b73f28f30372ca6d75b355bd9f11ca9b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49295262"
---
# <a name="managedebookassignment-resource-type"></a>managedEBookAssignment 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于为组分配电子书的属性。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[列出 managedEBookAssignments](../api/intune-books-managedebookassignment-list.md)|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 集合|列出 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象的属性和关系。|
|[获取 managedEBookAssignment](../api/intune-books-managedebookassignment-get.md)|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|读取 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象的属性和关系。|
|[创建 managedEBookAssignment](../api/intune-books-managedebookassignment-create.md)|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|创建新的 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象。|
|[删除 managedEBookAssignment](../api/intune-books-managedebookassignment-delete.md)|无|删除 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|
|[更新 managedEBookAssignment](../api/intune-books-managedebookassignment-update.md)|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|更新 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|实体的键。|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|电子图书的分配目标。|
|installIntent|[installIntent](../resources/intune-shared-installintent.md)|电子图书的安装意图。 可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBookAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  },
  "installIntent": "String"
}
```




