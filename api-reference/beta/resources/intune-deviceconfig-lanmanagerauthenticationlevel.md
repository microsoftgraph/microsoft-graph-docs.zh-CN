---
title: lanManagerAuthenticationLevel 枚举类型
description: LanManagerAuthenticationLevel 的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fd88deb7684301023a75905d12a59ce25bad750f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911992"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a>lanManagerAuthenticationLevel 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

LanManagerAuthenticationLevel 的可能值
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|lmAndNltm|0|发送 LM 和 NTLM 响应|
|lmNtlmAndNtlmV2|1|如果协商，发送 LM 和 NTLM 使用 NTLMv2 会话安全|
|lmAndNtlmOnly|2|发送 LM 和 NTLM 响应|
|lmAndNtlmV2|3|发送 LM 和 NTLMv2 响应|
|lmNtlmV2AndNotLm|4|发送 LM 和 NTLMv2 响应。 拒绝 LM|
|lmNtlmV2AndNotLmOrNtm|5|发送 LM 和 NTLMv2 响应。 拒绝 LM 和 NTLM|





