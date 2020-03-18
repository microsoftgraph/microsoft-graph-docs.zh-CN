---
title: eapFastConfiguration 枚举类型
description: EAP 快速配置的可用设置。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b70e2688473f9af93dcd3b0f0d4d05b77d81446f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791952"
---
# <a name="eapfastconfiguration-enum-type"></a>eapFastConfiguration 枚举类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

EAP 快速配置的可用设置。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|noProtectedAccessCredential|0|使用 EAP-FAST （无保护性访问凭据（PAC））。|
|useProtectedAccessCredential|1|使用受保护的访问凭据（PAC）。|
|useProtectedAccessCredentialAndProvision|双面|使用保护性接入身分凭证（PAC）和预配 PAC。|
|useProtectedAccessCredentialAndProvisionAnonymously|第三章|使用受保护的访问凭据（PAC）、预配 PAC，并以匿名方式执行此操作。|



