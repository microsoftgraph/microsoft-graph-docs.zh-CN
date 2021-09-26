---
title: 联机会议项目和权限
description: 了解联机会议项目以及提取这些项目所需的内容。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.date: 09/20/2021
ms.openlocfilehash: e8c220254d0e587225c3de0f371a3dc642490345
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59777304"
---
# <a name="online-meeting-artifacts-and-permissions"></a>联机会议项目和权限

联机会议项目是联机会议或实时事件期间生成的内容。 可以使用 Get [onlineMeeting](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true) 操作获取以下会议项目： 

- 联机会议（JSON 响应形式）的与会者报告。 出席报告具有以下特征：
  - 可用于实时事件外的会议
  - 仅在会议结束时可用
  - 只有会议组织者可以访问
- 实时事件的录制，形式为 60 秒后过期的下载链接。 录制具有以下特征：
  - 仅适用于实时事件
  - 仅在实时事件结束时可用
  - 只有实时事件组织者可以访问
- 实时事件的与会者报告，形式为 60 秒后过期的下载链接。 与会者报告具有以下特征：
  - 仅适用于实时事件
  - 仅在实时事件结束时可用
  - 只有实时事件组织者可以访问

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
