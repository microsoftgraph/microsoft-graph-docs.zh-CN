---
title: 呼叫记录概述
description: 通话记录可让你深入了解组织中发生的呼叫和会议。
author: williamlooney
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.openlocfilehash: 68dde7c3f2128f97e0019be69e48c7eef8c4c78a
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2022
ms.locfileid: "62804112"
---
# <a name="call-records-overview"></a>呼叫记录概述

通话记录提供了使用 Microsoft Teams 或 Skype for Business 时组织内发生的通话和联机会议的使用情况和诊断信息。 使用情况和诊断数据可用于生成企业自定义报告，以帮助监视采用情况或解决通话质量问题。

组织可以使用 Microsoft Graph [webhook](/graph/api/resources/webhooks.md) 订阅功能订阅对呼叫记录的更改，从而允许他们根据数据生成接近实时的报告，或对某些方案（如紧急呼叫）发出警报。

> **重要提示：** 在向应用程序授予 CallRecords.Read.All 权限时，请谨慎。 呼叫记录可提供业务运营的见解，因此可能是恶意参与者的目标。 仅为你信任的应用程序授予此权限，以满足你的数据保护要求。

## <a name="subscribe-to-call-records"></a>订阅通话记录

组织和合作伙伴通常拥有自己的工具来生成有关通话和联机会议的报告。 通过使用 webhook，他们可以在创建呼叫记录时收到连续的呼叫记录源。 利用此推送模型，组织和合作伙伴可以构建自己的实时报告解决方案。

## <a name="look-up-a-call-record-by-its-call-id"></a>按呼叫 ID 查找呼叫记录

应用程序可以按 [其 ID 检索](/graph/api/resources/callrecords-callrecord) 呼叫记录。 可以从 Webhook 通知确定此 ID，也可以从管理工具中检索此 ID。

## <a name="get-call-record-reports"></a>获取呼叫记录报告

使用 Microsoft Teams PSTN 网络连接到公用电话交换网 (PSTN) 通常需要跟踪此使用情况以了解相关成本。 [getPstnCalls](/graph/api/callrecords-callrecord-getpstncalls) 和 [getDirectRoutingCalls](/graph/api/callrecords-callrecord-getdirectroutingcalls) 函数以表格格式返回呼叫[](/graph/api/resources/callrecords-callrecord)记录数据的投影。

## <a name="see-also"></a>另请参阅

- [通话记录权限](./permissions-reference.md#call-records-permissions)
