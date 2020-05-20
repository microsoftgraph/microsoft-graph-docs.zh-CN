---
title: 在 Microsoft Graph 中选择 API 以创建和加入联机会议
description: 你可以灵活地创建将来或即时使用的会议
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: acbe97c2f5fb68547d5baabc4e7de0ef1de50641
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289848"
---
# <a name="choose-an-api-in-microsoft-graph-to-create-and-join-online-meetings"></a>在 Microsoft Graph 中选择 API 以创建和加入联机会议

Microsoft Graph 提供了两个可在 Microsoft 团队或 Skype 上安排和加入联机会议的 API 集：

- [日历 API](outlook-calendar-online-meetings.md)：使用[事件](/graph/api/resources/event)资源。
- [云通信 API](cloud-communications-online-meetings.md)：使用[onlineMeeting](/graph/api/resources/onlineMeeting)资源。

选择是在 Outlook 日历中方便地设置联机会议的方式，与会者加入并假设团队或 Skype UI 体验，而不是更丰富的编程集成团队或 Skype 功能，以实现更好的自定义应用程序体验或方案。

## <a name="considerations-when-choosing-an-api-for-your-scenario"></a>为方案选择 API 时的注意事项

选择与 Outlook 日历的简化的内置集成的日历 API，这将导致 Outlook 日历中出现联机会议事件：
- 编程支持：
  - 应用可以_直接在 outlook 日历中创建或更新作为联机会议的事件_，其中包含在 outlook 日历事件中插入的加入团队会议 blob。
  - 应用获取通过 Internet 加入会议或通过拨入的属性。
- 使用以编程方式创建的日历事件的与会者的 UI 体验与通过 Outlook UI 创建的任何事件都是完整的奇偶校验：
  - 与会者可以选择在网上或亲自开会。
  - 与会者可在加入团队-会议 blob 中单击，以通过 Internet 加入会议或通过拨入。
  - 与会者可以使用工作组的其他丰富功能，包括视频会议和会议厅（如果已配置）。

> **注意：** 与 Outlook 日历的集成假定管理员已为联机会议设置了 Outlook。 使用 API 之前，[请先验证](outlook-calendar-online-meetings.md#calendars-and-online-meeting-providers)支持。

选择云通信 API 以获得灵活性和更广泛的编程支持：
- 应用程序具有更大的灵活性，可进一步将 API 结果与业务线和其他应用集成。 API 与任何特定日历保持独立，不会在任何日历中创建事件。
- 应用可以为与会者提供以下功能：
  - 基于区域设置的联接信息（预览）。
  - 通过 Internet 或拨入方式加入会议。
  - 视频-会议。
  - 其他安全功能，如会议厅和自动参与者许可（预览）。
  - 将会议与 Microsoft 团队聊天相关联。

## <a name="comparing-the-apis"></a>比较 Api

下表详细介绍了 API 级别的差异。 


| 联机会议功能 | 日历 API （事件资源） | 云通信 API （onlineMeeting 资源）             |
|:-----------------------|:------------------------------|:-------------------------------------------------------------|
| 主要 API 成员 | [事件](/graph/api/resources/event)资源： <br>- **isOnlineMeeting**属性 <br>- [onlineMeetingInfo](/graph/api/resources/onlinemeetinginfo)类型的**onlineMeeting**属性 <br>- **onlineMeetingProvider**属性 <br> [日历](/graph/api/resources/calendar)资源： <br>- **allowedOnlineMeetingProviders**属性 <br>- **defaultOnlineMeetingProvider**属性 <br> | [onlineMeeting](/graph/api/resources/onlinemeeting)资源 <br> [audioConferencing](/graph/api/resources/audioconferencing)资源
| 与日历项目的集成 | <br> [Create](/graph/api/user-post-events) or [update](/graph/api/event-update) **event** API 自动将最终的 Outlook 日历[事件](/graph/api/resources/event)设置为联机会议。<br> 使用返回的 Outlook 日历**事件**的**isOnlineMeeting**、 **onlineMeeting**和**onlineMeetingProvider**属性。  | [创建](/graph/api/application-post-onlinemeetings)API 返回独立于特定日历类型的[onlineMeeting](/graph/api/resources/onlinemeeting)资源。 <br> 不会创建或更新任何 Outlook 事件。 <br> 将返回的**onlineMeeting**资源信息集成到适用于您的方案的应用程序体验中。 <br> 在预览中可用： [createOrGet](/graph/api/onlinemeeting-createorget?view=graph-rest-beta)联机会议，并使用返回的**externalId**属性简化在第三方日历中嵌入结果会议。 |
| 更改为脱机会议 | 否—一旦启用了联机加入的事件，就无法更新该**事件**以使其成为脱机会议。<br> 无法更改**onlineMeetingProvider**属性，也无法将**isOnlineMeeting**设置为 `false` ，以禁用联机会议。 | 否—创建**onlineMeeting**资源后，只能将其删除，但不能将其更改为脱机会议。 |
| 基于区域设置的联接信息 | 无直接 API 集成。 | `Accept-Language`创建联机会议时使用 HTTP 头（预览）。 <br> 请参阅[示例](/graph/api/application-post-onlinemeetings?view=graph-rest-beta#example-2-create-an-online-meeting-with-user-token)。 |
| 通过 Internet 进行联接（VoIP） | 通过**onlineMeeting**属性访问**joinUrl**。  | 使用**joinWebUrl**属性。 |
| 通过拨入进行连接 | 通过**onlineMeeting**属性，access： <br> **conferenceId**、 **quickDial**、**电话**、 **tollFreeNumbers**、 **tollNumber**。 | 通过**audioConferencing**属性，access： <br> - **conferenceId**、 **tollFreeNumber**、 **tollNumber**。<br> - 包含拨入信息以促进与第三方应用集成的可从外部访问的网页的**dialinUrl**属性。 |
| 通过视频会议（音频和视频）加入 | 无直接 API 集成。 | 使用**videoTeleconferenceId**属性。 |
| 会议会议厅和自动与会者进入联机会议 | 无直接 API 集成。<br> 在插入的加入团队-事件的会议 blob 中，如果管理员启用了会议会议厅，与会者可以单击**会议选项**链接来访问会议厅。 |API 将与会者与组织者的公司和联合公司以及其他与会者（包括匿名的）区分开来。  <br> 使用**autoAdmittedUsers**属性（预览）。  |
| 与团队聊天相关 | 无直接 API 集成。 | 使用**chatInfo**属性。 |


## <a name="see-also"></a>另请参阅
- [使用 Outlook 组织或参加联机会议](outlook-calendar-online-meetings.md)
- [使用云通信 API 创建或加入联机会议](cloud-communications-online-meetings.md)