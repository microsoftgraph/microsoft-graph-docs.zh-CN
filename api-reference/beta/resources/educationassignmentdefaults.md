---
title: educationAssignmentDefaults 资源类型
description: 指定类中创建的新作业所尊重的类级默认值
author: dipakboyed
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3b5804f98508d3dd2e4341f3834b5c9fd7068625
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/06/2022
ms.locfileid: "64684968"
---
# <a name="educationassignmentdefaults-resource-type"></a>educationAssignmentDefaults 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定类中创建的新作业所尊重的类级默认值。 如果调用方不想要默认行为，则可以继续指定每个作业创建的自定义值。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 educationAssignmentDefaults](../api/educationassignmentdefaults-get.md)|[educationAssignmentDefaults](../resources/educationassignmentdefaults.md)|读取 [educationAssignmentDefaults 对象的](../resources/educationassignmentdefaults.md) 属性和关系。|
|[更新 educationAssignmentDefaults](../api/educationassignmentdefaults-update.md)|[educationAssignmentDefaults](../resources/educationassignmentdefaults.md)|更新 [educationAssignmentDefaults 对象的](../resources/educationassignmentdefaults.md) 属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|educationAssignmentDefaults 的唯一标识符|
|addedStudentAction|educationAddedStudentAction|用于处理作业发布后添加的学生的课堂级默认行为。 可取值为：`none`、`assignIfOpen`。|
|addToCalendarAction| educationAddToCalendarOptions|用于控制在作业发布时向学生和教师日历添加作业的可选字段。 可能的值是： `none`、 `studentsAndPublisher`、 `studentsAndTeamOwners`、 `unknownFutureValue`和 `studentsOnly`。 请注意，必须使用`Prefer: include-unknown-enum-members`请求标头获取以下值 (此[可旋转枚举](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations)中的) ： `studentsOnly` 默认值为 `none`。|
|dueTime|TimeOfDay|截止时间字段的类级默认值。 默认值为 `23:59:00`。|
|notificationChannelUrl|String|将向其发送通知的默认Teams通道。 默认值为 `null`。|

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
  "id": "String (identifier)",
  "addedStudentAction": "none",
  "addToCalendarAction": "none",
  "dueTime": "23:59:00",
  "notificationChannelUrl": "https://graph.microsoft.com/beta/teams('id')/channels('id')"
}
```

