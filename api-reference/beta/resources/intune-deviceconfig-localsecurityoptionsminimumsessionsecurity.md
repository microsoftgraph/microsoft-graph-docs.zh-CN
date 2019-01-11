---
title: localSecurityOptionsMinimumSessionSecurity 枚举类型
description: LocalSecurityOptionsMinimumSessionSecurity 的可能值
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fb6912e7d3bba42364849165cceb28050ddacfae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833234"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a>localSecurityOptionsMinimumSessionSecurity 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

LocalSecurityOptionsMinimumSessionSecurity 的可能值
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|无|0|发送 LM 和 NTLM 响应|
|requireNtmlV2SessionSecurity|1|如果协商，发送 LM 和 NTLM 使用 NTLMv2 会话安全|
|require128BitEncryption|2|发送 LM 和 NTLM 响应|
|ntlmV2And128BitEncryption|3|发送 LM 和 NTLMv2 响应|





