---
title: localSecurityOptionsMinimumSessionSecurity 枚举类型
description: LocalSecurityOptionsMinimumSessionSecurity 的可能值
author: tfitzmac
ms.openlocfilehash: 5feabd9c84ec42f55bb45b952be5af834fd84498
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350629"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a>localSecurityOptionsMinimumSessionSecurity 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

LocalSecurityOptionsMinimumSessionSecurity 的可能值
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|发送 LM 和 NTLM 响应|
|requireNtmlV2SessionSecurity|1|如果协商，发送 LM 和 NTLM 使用 NTLMv2 会话安全|
|require128BitEncryption|2|发送 LM 和 NTLM 响应|
|ntlmV2And128BitEncryption|3|发送 LM 和 NTLMv2 响应|





