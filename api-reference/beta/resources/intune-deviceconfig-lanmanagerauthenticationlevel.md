---
title: lanManagerAuthenticationLevel 枚举类型
description: LanManagerAuthenticationLevel 的可能值
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6e8c7b3df6f515d3dad0d7619b6c0b755ad799d7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397454"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a>lanManagerAuthenticationLevel 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

LanManagerAuthenticationLevel 的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|lmAndNltm|0|发送 LM & NTLM 响应|
|lmNtlmAndNtlmV2|1|如果协商，发送 LM & NTLM 使用 NTLMv2 会话安全|
|lmAndNtlmOnly|2|发送 LM & 仅 NTLM 响应|
|lmAndNtlmV2|3|发送 LM & 仅 NTLMv2 响应|
|lmNtlmV2AndNotLm|4|发送 LM & 仅 NTLMv2 响应。 拒绝 LM|
|lmNtlmV2AndNotLmOrNtm|5|发送 LM & 仅 NTLMv2 响应。 拒绝 LM & NTLM|




