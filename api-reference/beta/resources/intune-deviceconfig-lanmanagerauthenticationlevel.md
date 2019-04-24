---
title: lanManagerAuthenticationLevel 枚举类型
description: LanManagerAuthenticationLevel 的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3b93f229661de3e2fbb28f764288983b2fd83bb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460490"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a>lanManagerAuthenticationLevel 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

LanManagerAuthenticationLevel 的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|lmAndNltm|0|发送 LM & NTLM 响应|
|lmNtlmAndNtlmV2|1|发送 LM & NTLM-使用 NTLMv2 会话安全性 (如果协商)|
|lmAndNtlmOnly|2 |仅发送 LM & NTLM 响应|
|lmAndNtlmV2|3 |仅发送 LM & NTLMv2 响应|
|lmNtlmV2AndNotLm|4 |仅发送 LM & NTLMv2 响应。 拒绝 LM|
|lmNtlmV2AndNotLmOrNtm|5|仅发送 LM & NTLMv2 响应。 拒绝 LM & NTLM|





