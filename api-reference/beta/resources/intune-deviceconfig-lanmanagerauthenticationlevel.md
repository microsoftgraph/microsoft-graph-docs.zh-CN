---
title: lanManagerAuthenticationLevel 枚举类型
description: LanManagerAuthenticationLevel 的可能值
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ff913766f41dfa3ec1a53c3a1ba37fc94cbc2b23
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59127086"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a>lanManagerAuthenticationLevel 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

LanManagerAuthenticationLevel 的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|lmAndNltm|0|发送 LM & NTLM 响应|
|lmNtlmAndNtlmV2|1|发送 LM & NTLM 使用 NTLMv2 会话安全性（如果已协商）|
|lmAndNtlmOnly|2|仅发送 LM & NTLM 响应|
|lmAndNtlmV2|3|仅发送 LM & NTLMv2 响应|
|lmNtlmV2AndNotLm|4 |仅发送 LM & NTLMv2 响应。 拒绝 LM|
|lmNtlmV2AndNotLmOrNtm|5 |仅发送 LM & NTLMv2 响应。 拒绝 LM & NTLM|



