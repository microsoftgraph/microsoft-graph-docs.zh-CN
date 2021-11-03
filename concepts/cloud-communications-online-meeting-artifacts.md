---
title: 联机会议项目和权限
description: 了解联机会议项目以及提取这些项目所需的内容。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.date: 09/20/2021
ms.openlocfilehash: 59d5bca4e8484d7965eeef44e44c08b7c67b09fb
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60685525"
---
# <a name="online-meeting-artifacts-and-permissions"></a>联机会议项目和权限

联机会议项目是联机会议或实时事件期间Microsoft Teams[的内容](/microsoftteams/teams-live-events/what-are-teams-live-events)。 可以使用 Get [onlineMeeting](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true) 操作获取以下会议项目：

- 联机会议（JSON 响应形式）的与会者报告。 出席报告具有以下特征：
  - 可用于实时事件Teams会议
  - 仅在会议结束时可用
  - 只有会议组织者可以访问
- 实时事件Teams，形式为 60 秒后过期的下载链接。 录制具有以下特征：
  - 仅适用于Teams活动
  - 仅在实时Teams结束时可用
  - 只有Teams事件组织者可以访问
- 实时事件的Teams报告，形式为 60 秒后过期的下载链接。 与会者报告具有以下特征：
  - 仅适用于Teams活动
  - 仅在实时Teams结束时可用
  - 只有Teams事件组织者可以访问

## <a name="permissions"></a>权限

以下权限可用于管理会议项目。

- 委派 (工作或学校帐户) - OnlineMeetingArtifact.Read.All
- Application - OnlineMeetingArtifact.Read.All

只有 _OnlineMeetingArtifact.Read.All_ 权限才能提取联机会议项目。 在 **2022** 年 1 月 15 日之前，您可以使用以下权限获取 beta 版中的会议项目：

- _OnlineMeeting.Read_
- _OnlineMeeting.ReadWrite_
- _OnlineMeeting.Read.All_
- _OnlineMeeting.ReadWrite.All_

在此日期之后， _需要 OnlineMeetingArtifact.Read.All_ 权限才能提取会议项目;将拒绝没有这些权限的请求。
