---
title: 云通信 API 中的联机会议项目和权限
description: 了解联机会议项目，例如出席情况报告和录制，以及使用 Microsoft Graph 云通信 API 提取这些项目所需的权限。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.date: 09/20/2021
ms.openlocfilehash: 019e88a0d3f5fb046c94e7074644a3a01a94ae14
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440987"
---
# <a name="online-meeting-artifacts-and-permissions"></a>联机会议项目和权限

联机会议项目是在线会议或 [Microsoft Teams 直播活动](/microsoftteams/teams-live-events/what-are-teams-live-events)期间生成的内容。 可以使用 [Get onlineMeeting](/graph/api/onlinemeeting-get) 操作获取以下会议项目：

- 联机会议的出席情况报告（以 JSON 响应的形式）。 出席情况报告具有以下特征：
  - 适用于 Teams 直播活动以外的会议
  - 仅当会议结束时才可用
  - 只有会议组织者才能访问
- Teams 实时事件的录制，其形式为下载链接，该链接将在 60 秒后过期。 录制具有以下特征：
  - 仅适用于 Teams 直播活动
  - 仅当 Teams 直播活动结束时才可用
  - 只有 Teams 直播活动组织者才能访问
- Teams 实时活动的与会者报告，其形式为下载链接，该链接将在 60 秒后过期。 与会者报表具有以下特征：
  - 仅适用于 Teams 直播活动
  - 仅当 Teams 直播活动结束时才可用
  - 只有 Teams 直播活动组织者才能访问

## <a name="permissions"></a>权限

以下权限可用于管理会议项目：

- 委派 (工作或学校帐户) - OnlineMeetingArtifact.Read.All
- 应用程序 - OnlineMeetingArtifact.Read.All

仅需要 _OnlineMeetingArtifact.Read.All_ 权限才能提取联机会议项目。 在 **2022 年 1 月 15** 日之前，可以使用以下权限在 beta 中获取会议项目：

- _OnlineMeeting.Read_
- _OnlineMeeting.ReadWrite_
- _OnlineMeeting.Read.All_
- _OnlineMeeting.ReadWrite.All_

该日期之后，需要 _OnlineMeetingArtifact.Read.All_ 权限才能提取会议项目;没有这些权限的请求将被拒绝。

## <a name="see-also"></a>另请参阅

- [云通信 API 概述](cloud-communications-concept-overview.md)