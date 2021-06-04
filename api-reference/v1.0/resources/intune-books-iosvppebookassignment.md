---
title: iosVppEBookAssignment 资源类型
description: 包含用于为组分配 iOS VPP 电子书的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6fcc47a65a521658c4cbb97eafd4e90d20f7198f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52742921"
---
# <a name="iosvppebookassignment-resource-type"></a>iosVppEBookAssignment 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于为组分配 iOS VPP 电子书的属性。


继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[List iosVppEBookAssignments](../api/intune-books-iosvppebookassignment-list.md)|[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 集合|列出 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象的属性和关系。|
|[Get iosVppEBookAssignment](../api/intune-books-iosvppebookassignment-get.md)|[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md)|读取 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象的属性和关系。|
|[Create iosVppEBookAssignment](../api/intune-books-iosvppebookassignment-create.md)|[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md)|创建新的 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象。|
|[Delete iosVppEBookAssignment](../api/intune-books-iosvppebookassignment-delete.md)|无|删除 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md)。|
|[Update iosVppEBookAssignment](../api/intune-books-iosvppebookassignment-update.md)|[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md)|更新 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|电子图书的分配目标。 继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|
|installIntent|[installIntent](../resources/intune-shared-installintent.md)|电子图书的安装意图。 继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)。 可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppEBookAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "String"
}
```




