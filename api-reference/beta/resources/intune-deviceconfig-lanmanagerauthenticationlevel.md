---
title: lanManagerAuthenticationLevel 枚举类型
description: LanManagerAuthenticationLevel 的可能值
ms.openlocfilehash: 9fb8113c4953a0cabcecfbc5303b9f62f685d5ca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041943"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a>lanManagerAuthenticationLevel 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

LanManagerAuthenticationLevel 的可能值
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|lmAndNltm|0|发送 LM 和 NTLM 响应|
|lmNtlmAndNtlmV2|1|如果协商，发送 LM 和 NTLM 使用 NTLMv2 会话安全|
|lmAndNtlmOnly|2|发送 LM 和 NTLM 响应|
|lmAndNtlmV2|3|发送 LM 和 NTLMv2 响应|
|lmNtlmV2AndNotLm|4|发送 LM 和 NTLMv2 响应。 拒绝 LM|
|lmNtlmV2AndNotLmOrNtm|5|发送 LM 和 NTLMv2 响应。 拒绝 LM 和 NTLM|





