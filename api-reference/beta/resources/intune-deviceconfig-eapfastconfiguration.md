---
title: eapFastConfiguration 枚举类型
description: EAP FAST 配置的可用设置。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1fa2c3c3a4cf0bc245ea7c9fbc4294d69215deee
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399386"
---
# <a name="eapfastconfiguration-enum-type"></a>eapFastConfiguration 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

EAP FAST 配置的可用设置。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|noProtectedAccessCredential|0|使用 EAP-FAST 不受保护的访问凭据 (PAC)。|
|useProtectedAccessCredential|1|使用受保护访问凭据 (PAC)。|
|useProtectedAccessCredentialAndProvision|2|使用受保护的访问凭据 (PAC) 和设置 pac。|
|useProtectedAccessCredentialAndProvisionAnonymously|3|使用受保护访问凭据 (PAC)，设置 PAC，并以匿名方式这样。|




