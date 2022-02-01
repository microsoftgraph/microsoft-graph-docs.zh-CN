---
title: meetingRegistration 资源类型
description: 包含有关联机会议注册的信息。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ab41bebd48947851721e2adc78a07f01fc522117
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/01/2022
ms.locfileid: "62291960"
---
# <a name="meetingregistration-resource-type"></a>meetingRegistration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含联机会议（如网络研讨会）的[Microsoft Teams详细信息](https://support.microsoft.com/office/get-started-with-teams-webinars-42f3f874-22dc-4289-b53f-bbc1a69013e3)。 

继承自 [meetingRegistrationBase](meetingregistrationbase.md)。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
| :----- | :---------- | :---------- |
|[创建](../api/meetingregistration-post.md) | [meetingRegistration](meetingregistration.md) | 创建并启用联机会议注册。 |
|[获取](../api/meetingregistration-get.md) | [meetingRegistration](meetingregistration.md) | 检索会议注册的详细信息。 |
|[更新](../api/meetingregistration-update.md) | [meetingRegistration](meetingregistration.md) | 更新会议注册的详细信息。 |
|[删除](../api/meetingregistration-delete.md) | [meetingRegistration](meetingregistration.md) | 禁用和删除联机会议注册。 |

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
| :------- | :--- | :---------- |
| allowedRegistrant | [meetingAudience](#meetingaudience-values) | 指定可注册会议的人。 |
| description | String | 会议说明。 |
| endDateTime | DateTime | 会议结束时间（UTC）。 |
| registrationPageViewCount | Int32 | 已访问注册页次数。 只读。 |
| registrationPageWebUrl | String | 注册页的 URL。 只读。 |
| 扬声器 | [meetingSpeaker](meetingSpeaker.md) 集合 | 会议发言人的信息。 |
| startDateTime | DateTime | 会议开始时间（UTC）。 |
| subject | String | 会议的主题。 |

### <a name="meetingaudience-values"></a>meetingAudience 值

| 值              | 说明 |
| ------------------ | ----------- |
| everyone           | 每个人都可以注册会议。 |
| 组织       | 组织者组织中的每个人都可以注册会议。 |
| unknownFutureValue | 可发展枚举 sentinel 值。 请勿使用。 |

## <a name="relationships"></a>关系

| 关系 | 类型 | 说明 |
| ------------ | ---- | ----------- |
| customQuestions | [meetingRegistrationQuestion](meetingRegistrationQuestion.md) 集合| 自定义注册问题。 |
| registrants | [meetingRegistrant](meetingRegistrant.md) 集合 | 联机会议注册人。 |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.meetingRegistration"
}-->

```json
{
  "allowedRegistrant": { "@odata.type": "microsoft.graph.meetingAudience" },
  "description": "String",
  "endDateTime": "String (timestamp)",
  "registrationPageViewCount": "Int32",
  "registrationPageWebUrl": "String",
  "speakers": [{ "@odata.type": "microsoft.graph.meetingSpeaker" }],
  "startDateTime": "String (timestamp)",
  "subject": "String",

  "customQuestions": [{ "@odata.type": "microsoft.graph.meetingRegistrationQuestion" }],
  "registrants": [{ "@odata.type": "microsoft.graph.meetingRegistrant" }]
}
```
