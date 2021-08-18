---
title: eapFastConfiguration 枚举类型
description: EAP-FAST的可用设置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3f3f6db981d29c2150beba9d391180248c9151188d97b2b6810cf6ae13e19285
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54227467"
---
# <a name="eapfastconfiguration-enum-type"></a>eapFastConfiguration 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

EAP-FAST的可用设置。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|noProtectedAccessCredential|0|使用 EAP-FAST无受保护的访问凭据 (PAC) 。|
|useProtectedAccessCredential|1 |使用受保护的访问凭据 (PAC) 。|
|useProtectedAccessCredentialAndProvision|2 |使用受保护的访问凭据 (PAC) 设置 PAC。|
|useProtectedAccessCredentialAndProvisionAnonymously|3 |使用受保护的访问凭据 (PAC) 设置 PAC，并匿名执行。|




