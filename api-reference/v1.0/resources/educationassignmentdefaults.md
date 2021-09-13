---
title: educationAssignmentDefaults 资源类型
description: 指定在类中创建的新作业所遵守的类级别默认值
author: sharad-sharma-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7a21494ca3bd039e0ac5ac28c5f02be3c802dea0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59021713"
---
# <a name="educationassignmentdefaults-resource-type"></a>educationAssignmentDefaults 资源类型

命名空间：microsoft.graph

指定在类中创建的新工作分配所遵守的类级别默认值。 

如果调用方不希望使用默认行为，可以继续为每个工作分配创建指定自定义值。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 educationAssignmentDefaults](../api/educationassignmentdefaults-get.md)|[educationAssignmentDefaults](../resources/educationassignmentdefaults.md)|读取 [educationAssignmentDefaults 对象的属性和](../resources/educationassignmentdefaults.md) 关系。|
|[更新 educationAssignmentDefaults](../api/educationassignmentdefaults-update.md)|[educationAssignmentDefaults](../resources/educationassignmentdefaults.md)|更新 [educationAssignmentDefaults 对象](../resources/educationassignmentdefaults.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|addedStudentAction|educationAddedStudentAction|用于处理作业发布后添加的学生的课堂级别默认行为。 可取值为：`none`、`assignIfOpen`。|
|dueTime|TimeOfDay|"到期时间"字段的类级别默认值。 默认值为 `23:59:00`。|
|notificationChannelUrl|String|默认Teams通知将发送到的频道。 默认值为 `null`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationAssignmentDefaults",
  "openType": false
}
-->
``` json
{
  "addedStudentAction": "String",
  "dueTime": "String (timestamp)",
  "notificationChannelUrl": "String"
}
```

