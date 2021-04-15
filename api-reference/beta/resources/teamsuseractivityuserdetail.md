---
title: teamsUserActivityUserDetail 资源类型
description: 表示有关用户 Microsoft Teams 用户活动的详细信息。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4afa7f17acac13eaa1c517953517fcfbe344aaa7
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766432"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a>teamsUserActivityUserDetail 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关用户 Microsoft Teams 用户活动的详细信息。

## <a name="properties"></a>属性

| 属性                                 | 类型              | 说明                                                  |
| :--------------------------------------- | :---------------- | ------------------------------------------------------------ |
| reportRefreshDate                        | 日期              | 内容的最新日期。                              |
| userPrincipalName                        | String            | 用户的用户主体名称 (UPN)。 UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。 按照惯例，此名称应映射到用户的电子邮件名称。 常规格式是 alias@domain，其中，domain 必须位于租户的已验证域集合中。 创建用户时此属性是必需的。 |
| isLicensed                               | Boolean           | 是否已为用户分配 Teams 许可证。          |
| lastActivityDate                         | 日期              | 用户上次参与 Microsoft Teams 活动的日期。 |
| isDeleted                                | Boolean           | 此用户是已删除还是软删除。          |
| deletedDate                              | 日期              | 删除操作发生的日期。 如果用户尚未删除，则默认值为"null"。 |
| assignedProducts                         | String 集合 | 用户分配的产品。                             |
| teamChatMessageCount                     | Int64             | 用户在团队聊天中发布的唯一消息数。 |
| privateChatMessageCount                  | Int64             | 用户在私人聊天中发布的唯一消息数。 |
| callCount                                | Int64             | 用户参与的 1：1 呼叫数。       |
| meetingCount                             | Int64             | 用户参与的联机会议数。 |
| meetingsOrganizedCount                   | Int64             | 用户组织的一次性计划会议、定期会议、临时会议和未分类会议的总和。 |
| meetingsAttendedCount                    | Int64             | 用户参与的一次性计划、定期、临时和未分类会议的总和。 |
| adHocMeetingsOrganizedCount              | Int64             | 用户组织的临时会议的数量。              |
| adHocMeetingsAttendedCount               | Int64             | 用户参与临时会议的数量。        |
| scheduledOneTimeMeetingsOrganizedCount   | Int64             | 用户组织的一次计划会议的数量。  |
| scheduledOneTimeMeetingsAttendedCount    | Int64             | 用户参与的一次计划会议的数量。 |
| scheduledRecurringMeetingsOrganizedCount | Int64             | 用户组织的定期会议数。           |
| scheduledRecurringMeetingsAttendedCount  | Int64             | 用户参与的定期会议的数量。 |
| audioDuration                            | 持续时间          | 用户参与的音频持续时间。                     |
| videoDuration                            | 持续时间          | 用户参与的视频持续时间。                     |
| screenShareDuration                      | 持续时间          | 用户参与的屏幕共享持续时间。            |
| hasOtherAction                           | Boolean           | 用户处于活动状态，但执行了除报告中提供的公开操作类型外的其他活动 (发送或回复频道消息和聊天消息、安排或参与一对一通话和会议) 。 示例操作包括用户更改 Teams 状态或 Teams 状态消息或打开频道消息帖子但不回复的情况。 |
| reportPeriod                             | String            | 报告涵盖的天数。                        |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "isLicensed": true, 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "assignedProducts": ["String"],
  "teamChatMessageCount": 1024, 
  "privateChatMessageCount": 1024, 
  "callCount": 1024, 
  "meetingCount": 1024, 
  "meetingsOrganizedCount": 1024, 
  "meetingsAttendedCount": 1024, 
  "adHocMeetingsOrganizedCount": 1024, 
  "adHocMeetingsAttendedCount": 1024, 
  "scheduledOneTimeMeetingsOrganizedCount": 1024, 
  "scheduledOneTimeMeetingsAttendedCount": 1024, 
  "scheduledRecurringMeetingsOrganizedCount": 1024, 
  "scheduledRecurringMeetingsAttendedCount": 1024, 
  "audioDuration": "Duration", 
  "videoDuration": "Duration", 
  "screenShareDuration": "Duration", 
  "hasOtherAction": true, 
  "reportPeriod": "String"
}
```


