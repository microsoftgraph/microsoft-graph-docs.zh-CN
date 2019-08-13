---
title: localSecurityOptionsMinimumSessionSecurity 枚举类型
description: LocalSecurityOptionsMinimumSessionSecurity 的可能值
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8dc6a96f5dda3cdba9ea3a57507bef4f32edc5a8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325524"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a>localSecurityOptionsMinimumSessionSecurity 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

LocalSecurityOptionsMinimumSessionSecurity 的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|发送 LM & NTLM 响应|
|requireNtmlV2SessionSecurity|1|发送 LM & NTLM-如果协商, 则使用 NTLMv2 会话安全性|
|require128BitEncryption|双面|仅发送 LM & NTLM 响应|
|ntlmV2And128BitEncryption|第三章|仅发送 LM & NTLMv2 响应|



