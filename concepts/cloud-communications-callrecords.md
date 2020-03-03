---
title: 呼叫记录概述
description: 呼叫记录可帮助您深入了解组织内发生的呼叫和会议。
author: stephenjust
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 4999f4b0d479b6e618055d39a3fecab340deb650
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394637"
---
# <a name="call-records-overview"></a>呼叫记录概述

呼叫记录提供了使用 Microsoft 团队或 Skype for Business 时在组织内发生的呼叫和联机会议的使用和诊断信息。 可以使用使用率和诊断数据来为您的企业生成自定义报告，以帮助监控采用或解决呼叫质量问题。

组织可以使用 Microsoft Graph [webhook 订阅](/graph/api/resources/webhooks?view=graph-rest-beta)功能订阅对呼叫记录所做的更改，从而允许他们生成来自数据的近实时报告或在某些情况下（如紧急呼叫）发出警报。

> **重要说明：** 授予对应用程序的 CallRecords 权限时，请务必谨慎。 呼叫记录可提供业务运营的见解，因此可以成为恶意参与者的目标。 仅向你信任的应用程序授予此权限，以满足你的数据保护要求。

## <a name="subscribe-to-call-records"></a>订阅呼叫记录

组织和合作伙伴通常拥有自己的工具来生成有关呼叫和联机会议的报告。 使用 webhook，他们可以在创建呼叫记录时接收连续的呼叫记录源。 此推送模型使组织和合作伙伴能够构建自己的实时报告解决方案。

## <a name="look-up-a-call-record-by-its-call-id"></a>按呼叫 ID 查找呼叫记录

应用程序可以按其 ID 检索[呼叫记录](/graph/api/resources/callrecords-callrecord?view=graph-rest-beta)。 可以从 webhook 通知或从管理工具检索到此 ID。

## <a name="see-also"></a>另请参阅

- [呼叫记录权限](/graph/permissions-reference#call-records-permissions)
