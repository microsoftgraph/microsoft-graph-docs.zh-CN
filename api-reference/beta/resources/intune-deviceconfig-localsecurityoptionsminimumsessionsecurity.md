---
title: localSecurityOptionsMinimumSessionSecurity 枚举类型
description: LocalSecurityOptionsMinimumSessionSecurity 的可能值
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d3ecff15416ff3d313840d7b3a0ca33c2ef83e3b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033684"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a>localSecurityOptionsMinimumSessionSecurity 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

LocalSecurityOptionsMinimumSessionSecurity 的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|发送 LM & NTLM 响应|
|requireNtmlV2SessionSecurity|1|发送 LM & NTLM 使用 NTLMv2 会话安全性（如果已协商）|
|require128BitEncryption|2|仅发送 LM & NTLM 响应|
|ntlmV2And128BitEncryption|3|仅发送 LM & NTLMv2 响应|



