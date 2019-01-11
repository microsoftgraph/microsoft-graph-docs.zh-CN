---
title: eapFastConfiguration 枚举类型
description: EAP FAST 配置的可用设置。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 499d6595980bcb6bca1ea93687399e8988a3bed7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811086"
---
# <a name="eapfastconfiguration-enum-type"></a>eapFastConfiguration 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

EAP FAST 配置的可用设置。
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|noProtectedAccessCredential|0|使用 EAP-FAST 不受保护的访问凭据 (PAC)。|
|useProtectedAccessCredential|1|使用受保护访问凭据 (PAC)。|
|useProtectedAccessCredentialAndProvision|2|使用受保护的访问凭据 (PAC) 和设置 pac。|
|useProtectedAccessCredentialAndProvisionAnonymously|3|使用受保护访问凭据 (PAC)，设置 PAC，并以匿名方式这样。|





