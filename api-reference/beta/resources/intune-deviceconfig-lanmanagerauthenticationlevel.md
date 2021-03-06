---
title: lanManagerAuthenticationLevel 枚举类型
description: LanManagerAuthenticationLevel 的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7fd08d1ce3dd40e3c60c8cbc42985f4014e1f332
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49269026"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a>lanManagerAuthenticationLevel 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

LanManagerAuthenticationLevel 的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|lmAndNltm|0|发送 LM & NTLM 响应|
|lmNtlmAndNtlmV2|1|发送 LM & NTLM-如果协商，则使用 NTLMv2 会话安全性|
|lmAndNtlmOnly|双面|仅发送 LM & NTLM 响应|
|lmAndNtlmV2|第三章|仅发送 LM & NTLMv2 响应|
|lmNtlmV2AndNotLm|4 |仅发送 LM & NTLMv2 响应。 拒绝 LM|
|lmNtlmV2AndNotLmOrNtm|5 |仅发送 LM & NTLMv2 响应。 拒绝 LM & NTLM|




