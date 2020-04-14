---
title: localSecurityOptionsMinimumSessionSecurity 枚举类型
description: LocalSecurityOptionsMinimumSessionSecurity 的可能值
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f5d7e052d5b814bb10d3c0851683deccdf9f9f5f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439971"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a>localSecurityOptionsMinimumSessionSecurity 枚举类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

LocalSecurityOptionsMinimumSessionSecurity 的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|发送 LM & NTLM 响应|
|requireNtmlV2SessionSecurity|1|发送 LM & NTLM-如果协商，则使用 NTLMv2 会话安全性|
|require128BitEncryption|双面|仅发送 LM & NTLM 响应|
|ntlmV2And128BitEncryption|第三章|仅发送 LM & NTLMv2 响应|



