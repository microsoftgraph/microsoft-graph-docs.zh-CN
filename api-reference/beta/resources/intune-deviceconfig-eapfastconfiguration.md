---
title: eapFastConfiguration 枚举类型
description: EAP FAST 配置的可用设置。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 65165929d388ed57f2651a0d277996e56d2f046e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954454"
---
# <a name="eapfastconfiguration-enum-type"></a>eapFastConfiguration 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

EAP FAST 配置的可用设置。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|noProtectedAccessCredential|0|使用 EAP-FAST 不受保护的访问凭据 (PAC)。|
|useProtectedAccessCredential|1|使用受保护访问凭据 (PAC)。|
|useProtectedAccessCredentialAndProvision|2|使用受保护的访问凭据 (PAC) 和设置 pac。|
|useProtectedAccessCredentialAndProvisionAnonymously|3|使用受保护访问凭据 (PAC)，设置 PAC，并以匿名方式这样。|





