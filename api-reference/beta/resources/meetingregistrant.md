---
title: meetingRegistrant 资源类型
description: 表示已注册联机会议的会议注册人。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: dbc90ecc79258ad150077d474fcdd8d4b29f6db6
ms.sourcegitcommit: c3f849e5a052b1926373a4b316ec303250e6d09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/15/2021
ms.locfileid: "60369456"
---
# <a name="meetingregistrant-resource-type"></a>meetingRegistrant 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示已注册联机会议的会议 [注册人](onlinemeeting.md)。

## <a name="methods"></a>方法

| 方法 | 返回类型 | Description |
| :----- | :---------- | :---------- |
|[List](../api/meetingregistration-list-registrants.md) | [meetingRegistrant](meetingregistrant.md) | 列出已注册会议的所有注册人。 |
|[Create](../api/meetingregistration-post-registrants.md) | [meetingRegistrant](meetingregistrant.md) | 在联机会议中注册注册人。 |
|[删除](../api/meetingregistrant-delete.md) | [meetingRegistrant](meetingregistrant.md) | 从联机会议取消注册注册。 |

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
| :------- | :--- | :---------- |
| customQuestionAnswers | [customQuestionAnswer](customQuestionAnswer.md) 集合 | 注册人对自定义问题的答案。 |
| email | String | 注册人的电子邮件地址。 |
| firstName | String | 注册人的名字。 |
| id | String | 注册人 ID。 只读。 |
| joinWebUrl | String | 注册人加入会议的唯一 Web URL。 只读。 |
| lastName | String | 注册表项的姓氏。 |
| registrationDateTime | String | 注册人注册会议的时间（UTC）。 只读。 |
| status | [meetingRegistrantStatus](#meetingregistrantstatus-values) | 注册人注册状态。 只读。 |

### <a name="meetingregistrantstatus-values"></a>meetingRegistrantStatus 值

| 值              | 说明 |
|--------------------|-------------|
| registered | 注册人已注册会议。 |
| canceled | 注册者已取消注册。 |
| processing | 指示状态正在处理的临时状态。 |
| unknownFutureValue | 可发展枚举 sentinel 值。 请勿使用。 |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.meetingRegistrant"
}-->

```json
{
  "id": "String",
  "firstName": "String (timestamp)",
  "email": "String",
  "lastName": "String",
  "joinWebUrl": "String",
  "registrationDateTime": "String (timestamp)",
  "status": { "@odata.type": "microsoft.graph.meetingRegistrantStatus" },
  "customQuestionAnswers": [{ "@odata.type": "microsoft.graph.customQuestionAnswer" }]
}
```
