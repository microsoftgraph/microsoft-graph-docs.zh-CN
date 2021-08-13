---
title: managedEBookAssignment 资源类型
description: 包含用于为组分配电子书的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c8c3eac1dc144e1baf38f1c9abe74b19e0491bb7c36e8aeee764eceaadd73e2c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180738"
---
# <a name="managedebookassignment-resource-type"></a>managedEBookAssignment 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于为组分配电子书的属性。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 managedEBookAssignments](../api/intune-books-managedebookassignment-list.md)|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 集合|列出 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象的属性和关系。|
|[获取 managedEBookAssignment](../api/intune-books-managedebookassignment-get.md)|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|读取 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象的属性和关系。|
|[创建 managedEBookAssignment](../api/intune-books-managedebookassignment-create.md)|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|创建新的 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象。|
|[删除 managedEBookAssignment](../api/intune-books-managedebookassignment-delete.md)|无|删除 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|
|[更新 managedEBookAssignment](../api/intune-books-managedebookassignment-update.md)|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|更新 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
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
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
  },
  "installIntent": "String"
}
```




