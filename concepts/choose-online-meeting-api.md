---
title: 在 Microsoft Graph 中选择 API 以创建和加入联机会议
description: 你可以灵活地创建将来或即时举行的会议
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: dd0bd14b30570afdfd442043cea4983ac98d1284
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59127939"
---
# <a name="choose-an-api-in-microsoft-graph-to-create-and-join-online-meetings"></a>在 Microsoft Graph 中选择 API 以创建和加入联机会议

Microsoft Graph 提供了两个 API 集，可在 Microsoft Teams 或 Skype 上安排和加入联机会议：

- [日历 API](outlook-calendar-online-meetings.md)：使用 [event](/graph/api/resources/event) 资源。
- [云通信 API](cloud-communications-online-meetings.md)：使用 [onlineMeeting](/graph/api/resources/onlineMeeting) 资源。

选择如下所示：
- 一种简便的编程方法，可在 Outlook 日历中设置一个联机会议，与会者可在该日历中单击加入会议，并在 Teams 或 Skype 中继续其体验。
- 在应用中，可通过更丰富的编程方式集成 Teams 或 Skype 功能，实现更好的自定义体验。

## <a name="considerations-when-choosing-an-api-for-your-scenario"></a>为方案选择 API 时的注意事项

选择日历 API，以获得与 Outlook 日历的简化内置集成，从而在 Outlook 日历中生成联机会议事件：
- 编程支持：
  - 应用可以 _在 Outlook 日历中作为联机会议直接创建或更新事件_，并在 Outlook 日历事件中插入一个“加入 Teams 会议”blob。
  - 应用可通过 Internet 或拨号方式获取用于加入会议的属性。
- 与会者的以编程方式创建的日历事件 UI 体验与通过 Outlook UI 创建的任何事件完全相同：
  - 与会者可以选择联机或亲自出席会议。
  - 与会者可以单击“加入 Teams 会议”blob 以通过 Internet 或拨号方式加入会议。
  - 如果已配置，则与会者可使用 Teams 的其他丰富功能（包括视频会议和会议厅）。

> **注意：** 与 Outlook 日历集成假设管理员已在 Outlook 中设置了联机会议。 使用 API 前，请[验证](/microsoftteams/exchange-teams-interact)支持。

选择云通信 API 以获得灵活性和更广泛的编程支持：
- 应用具有更大的灵活性，可以进一步将 API 结果与业务线和其他应用集成。 该 API 与任何特定日历保持分离，并且不会在任何日历中创建事件。
- 应用可为与会者提供以下功能：
  - 基于区域设置的加入信息。
  - 通过 Internet 或拨号方式加入会议。
  - 视频会议。
  - 其他安全功能（如会议厅）和自动与会者许可（预览）。
  - 将会议与 Microsoft Teams 聊天相关联。

## <a name="comparing-the-apis"></a>比较 API

下表详细介绍了 API 级别的区别。 


| 联机会议功能 | 日历 API（事件资源） | 云通信 API（onlineMeeting 资源）             |
|:-----------------------|:------------------------------|:-------------------------------------------------------------|
| 主要 API 成员 | [事件](/graph/api/resources/event)资源： <br>- **isOnlineMeeting** 属性 <br>- [onlineMeetingInfo](/graph/api/resources/onlinemeetinginfo) 类型的 **onlineMeeting** 属性 <br>- **onlineMeetingProvider** 属性 <br> [日历](/graph/api/resources/calendar)资源： <br>- **allowedOnlineMeetingProviders** 属性 <br>- **defaultOnlineMeetingProvider** 属性 <br> | [联机会议](/graph/api/resources/onlinemeeting)资源 <br> [音频会议](/graph/api/resources/audioconferencing)资源
| 与日历项目的集成 | <br>- [创建](/graph/api/user-post-events)或 [更新](/graph/api/event-update)**事件** API 会自动将生成的 Outlook 日历 [事件](/graph/api/resources/event)设置为联机会议。<br>-使用返回的 Outlook 日历 **事件** 的 **isOnlineMeeting**、**onlineMeeting** 和 **onlineMeetingProvider** 属性。  | - [创建](/graph/api/application-post-onlinemeetings) API 可返回与特定日历类型无关的[联机会议](/graph/api/resources/onlinemeeting)资源。 <br>- 不会创建或更新任何 Outlook 事件。 <br>- 将返回的 **联机会议** 资源信息集成到适合你的方案的应用体验中。 <br>- 使用 [createOrGet](/graph/api/onlinemeeting-createorget?view=graph-rest-beta) 返回具有指定 **externalId** 值的联机会议，或者创建一个外部值（如果不存在），以简化将生成的会议嵌入到第三方日历中的过程。 |
| 更改为脱机会议 | - 否 - 一旦启用了用于联机加入的 **事件**，就不能更新该事件以使其成为脱机会议。<br>- 不能更改 **onlineMeetingProvider** 属性，也不能将 **isOnlineMeeting** 设置为 `false` 以禁用联机会议。 | 否 - 创建 **联机会议** 资源后，只能删除它，而不能将其更改为脱机会议。 |
| 基于区域设置的加入信息 | 无直接 API 集成。 | - 创建联机会议时，请使用 `Accept-Language` HTTP 标头。 <br>- 请参阅[示例](/graph/api/application-post-onlinemeetings?view=graph-rest-beta#example-2-create-an-online-meeting-with-user-token)。 |
| 通过 Internet 加入 (VoIP) | 通过 **onlineMeeting** 属性访问 **joinUrl**。  | 使用 **joinWebUrl** 属性。 |
| 通过拨号方式加入 | 通过 **onlineMeeting** 属性访问： <br>- **conferenceId**、**quickDial**、**phones**、**tollFreeNumbers**、**tollNumber**。 |通过 **audioConferencing** 属性访问： <br> - **conferenceId**、**tollFreeNumber**、**tollNumber**。<br> - **dialinUrl** 用于可在外部访问的网页，其包含拨入信息，便于与第三方应用集成。 |
| 通过视频会议（音频和视频）加入 | 无直接 API 集成。 | 使用 **videoTeleconferenceId** 属性。 |
| 会议厅和自动准许与会者加入联机会议 | - 无直接 API 集成。<br>- 在事件的已注入“加入 Teams 会议”blob 中，如果管理员启用了“**会议选项**”链接，则与会者可以单击该链接来访问会议厅。 |- API 将来自组织者所在公司和联合公司的与会者以及其他与会者（包括匿名与会者）区分开。  <br>- 使用 **autoAdmittedUsers** 属性（预览）。  |
| 与 Teams 聊天相关 | 无直接 API 集成。 | 使用 **chatInfo** 属性。 |


## <a name="see-also"></a>另请参阅
- [在 Outlook 日历中将事件启用为联机会议](outlook-calendar-online-meetings.md)
- [使用云通信 API 创建或加入联机会议](cloud-communications-online-meetings.md)
