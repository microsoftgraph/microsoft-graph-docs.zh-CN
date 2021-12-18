---
title: educationAssignmentDefaults 资源类型
description: 指定在类中创建的新作业所遵守的类级别默认值
author: cristobal-buenrostro
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 620798d001df51bff352bcca4dce891a76f22cea
ms.sourcegitcommit: 15dd0e98e69f872ed5a709600608b244759b0967
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2021
ms.locfileid: "61567389"
---
# <a name="educationassignmentdefaults-resource-type"></a>educationAssignmentDefaults 资源类型

命名空间：microsoft.graph

指定在类中创建的新工作分配所遵守的类级别默认值。 

如果调用方不希望使用默认行为，可以继续为每个工作分配创建指定自定义值。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 educationAssignmentDefaults](../api/educationassignmentdefaults-get.md)|[educationAssignmentDefaults](../resources/educationassignmentdefaults.md)|读取 [educationAssignmentDefaults 对象的属性和](../resources/educationassignmentdefaults.md) 关系。|
|[更新 educationAssignmentDefaults](../api/educationassignmentdefaults-update.md)|[educationAssignmentDefaults](../resources/educationassignmentdefaults.md)|更新 [educationAssignmentDefaults 对象](../resources/educationassignmentdefaults.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|addedStudentAction|educationAddedStudentAction|用于处理作业发布后添加的学生的课堂级别默认行为。 可取值为：`none`、`assignIfOpen`。|
|addToCalendarAction| educationAddToCalendarOptions|可选字段，用于控制在作业发布时将作业添加到学生和教师的日历。 可能的值是 `none` `studentsAndPublisher` ：、、、 `studentsAndTeamOwners` `unknownFutureValue` 和 `studentsOnly` 。 请注意，必须使用此可变化枚举 (请求) 获取以下 `Prefer: include-unknown-enum-members` [值](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations) `studentsOnly` ： 。 默认值为 `none`。|
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
  "addToCalendarAction": "educationAddToCalendarOptions",  
  "dueTime": "String (timestamp)",
  "notificationChannelUrl": "String"
}
```

