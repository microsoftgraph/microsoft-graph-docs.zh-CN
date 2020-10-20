---
title: 呼叫记录概述
description: 呼叫记录可帮助您深入了解组织内发生的呼叫和会议。
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 11ca92e183531e133f5df20ec6a0d0e935487322
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601445"
---
# <a name="call-records-overview"></a>呼叫记录概述

通话记录提供了使用 Microsoft Teams 或 Skype for Business 时组织内发生的通话和联机会议的使用情况和诊断信息。 可以使用使用率和诊断数据来为您的企业生成自定义报告，以帮助监控采用或解决呼叫质量问题。

组织可以使用 Microsoft Graph [webhook 订阅](/graph/api/resources/webhooks?view=graph-rest-1.0) 功能订阅对呼叫记录所做的更改，从而允许他们生成来自数据的近实时报告或在某些情况下（如紧急呼叫）发出警报。

> **重要说明：** 授予对应用程序的 CallRecords 权限时，请务必谨慎。 呼叫记录可提供业务运营的见解，因此可以成为恶意参与者的目标。 仅为你信任的应用程序授予此权限，以满足你的数据保护要求。

## <a name="subscribe-to-call-records"></a>订阅呼叫记录

组织和合作伙伴通常拥有自己的工具来生成有关呼叫和联机会议的报告。 使用 webhook，他们可以在创建呼叫记录时接收连续的呼叫记录源。 此推送模型使组织和合作伙伴能够构建自己的实时报告解决方案。

## <a name="look-up-a-call-record-by-its-call-id"></a>按呼叫 ID 查找呼叫记录

应用程序可以按其 ID 检索 [呼叫记录](/graph/api/resources/callrecords-callrecord?view=graph-rest-1.0) 。 可以从 webhook 通知或从管理工具检索到此 ID。

## <a name="get-call-record-reports"></a>获取呼叫记录报告

使用 Microsoft 团队连接到公共交换电话网络 (PSTN) 的组织通常需要跟踪此使用情况，以了解相关的成本。 [GetPstnCalls](/graph/api/callrecords-callrecord-getpstncalls?view=graph-rest-beta)和[getDirectRoutingCalls](/graph/api/callrecords-callrecord-getdirectroutingcalls?view=graph-rest-beta)函数以表格格式返回[呼叫记录](/graph/api/resources/callrecords-callrecord?view=graph-rest-beta)数据的投影。

## <a name="see-also"></a>另请参阅

- [通话记录权限](./permissions-reference.md#call-records-permissions)