---
title: 云通信 API 中的呼叫记录
description: 深入了解使用 Microsoft Teams 或 Skype for Business 时组织内发生的呼叫和联机会议。
author: williamlooney
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.openlocfilehash: dc1c071ed6de21325fe154cc0a20f75e497d28c5
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436339"
---
# <a name="call-records"></a>通话记录

通话记录提供了使用 Microsoft Teams 或 Skype for Business 时组织内发生的通话和联机会议的使用情况和诊断信息。 可以使用使用情况和诊断数据为业务生成自定义报告，以帮助监视采用情况或排查呼叫质量问题。

组织可以使用 Microsoft Graph [Webhook 订阅](/graph/api/resources/webhooks) 功能订阅调用记录的更改，从而允许他们从数据生成近实时报告，或针对某些情况（如紧急呼叫）发出警报。

> [!IMPORTANT]
> 向应用程序授予 CallRecords.Read.All 权限时，请使用自由裁量权。 呼叫记录可以提供有关业务运营的见解，因此可以成为恶意行为者的目标。 仅为你信任的应用程序授予此权限，以满足你的数据保护要求。

## <a name="subscribe-to-call-records"></a>订阅呼叫记录

组织和合作伙伴通常有自己的工具来生成有关电话和联机会议的报告。 使用 Webhook，他们可以在创建呼叫记录时接收呼叫记录的连续源。 此推送模型使组织和合作伙伴能够构建自己的实时报告解决方案。

## <a name="look-up-a-call-record-by-its-call-id"></a>按呼叫 ID 查找呼叫记录

应用程序可以按其 ID 检索 [呼叫记录](/graph/api/resources/callrecords-callrecord) 。 此 ID 可以从 Webhook 通知中确定，也可以从管理工具中检索。

## <a name="get-call-record-reports"></a>获取呼叫记录报告

使用 Microsoft Teams 连接到公共交换电话网络 (PSTN) 的组织通常希望跟踪此使用情况，以了解相关成本。 [getPstnCalls](/graph/api/callrecords-callrecord-getpstncalls) 和 [getDirectRoutingCalls 函](/graph/api/callrecords-callrecord-getdirectroutingcalls)数以表格格式返回[调用记录](/graph/api/resources/callrecords-callrecord)数据的投影。

## <a name="see-also"></a>另请参阅

- [通话记录权限](./permissions-reference.md#call-records-permissions)
- [云通信 API 概述](cloud-communications-concept-overview.md)
