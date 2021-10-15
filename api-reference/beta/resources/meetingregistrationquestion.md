---
title: meetingRegistrationQuestion 资源类型
description: 代表与 meetingRegistration 关联的自定义注册问题，而不是名字、姓氏和电子邮件地址。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 42645be07a3540294906cb03fb7b28c080bbd0ed
ms.sourcegitcommit: c3f849e5a052b1926373a4b316ec303250e6d09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/15/2021
ms.locfileid: "60370337"
---
# <a name="meetingregistrationquestion-resource-type"></a>meetingRegistrationQuestion 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表与 [meetingRegistration](meetingRegistration.md)关联的自定义注册问题，而不是名字、姓氏和电子邮件地址。

## <a name="methods"></a>方法

| 方法 | 返回类型 | Description |
| :----- | :---------- | :---------- |
|[List](../api/meetingregistration-list-customquestions.md) | [meetingRegistrationQuestion](meetingregistrationquestion.md) 集合 | 列出所有自定义注册问题。 |
|[Create](../api/meetingregistration-post-customquestions.md) | [meetingRegistrationQuestion](meetingregistrationquestion.md) | 创建自定义注册问题。 |
|[Get](../api/meetingregistrationquestion-get.md) | [meetingRegistrationQuestion](meetingregistrationquestion.md) | 获取自定义注册问题。 |
|[更新](../api/meetingregistrationquestion-update.md) | [meetingRegistrationQuestion](meetingregistrationquestion.md) | 更新自定义注册问题。 |
|[删除](../api/meetingregistrationquestion-delete.md) | [meetingRegistrationQuestion](meetingregistrationquestion.md) | 删除自定义注册问题。 |

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
| :------- | :--- | :---------- |
| answerInputType | [answerInputType](#answerinputtype-values) | 回答自定义注册问题的输入类型。 |
| answerOptions | String 集合 | **answerInputType** 为 时回答选项 `radioButton` 。 |
| displayName | String | 自定义注册问题的显示名称。 |
| id | String | 自定义注册问题的 ID。 只读。 |
| isRequired | Boolean | 指示该问题是否是必需的。 默认值为 `false`。 |

### <a name="answerinputtype-values"></a>answerInputType 值

| 值              | 说明 |
|--------------------|-------------|
| text | 问题接受单行文本答案。 |
| radioButton | 问题接受从单选按钮选择的答案。 |
| unknownFutureValue | 可发展枚举 sentinel 值。 请勿使用。 |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.meetingRegistrationQuestion"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "isRequired": "Boolean",
  "answerInputType": { "@odata.type": "microsoft.graph.answerInputType" },
  "answerOptions": [ "String" ],
}
```
