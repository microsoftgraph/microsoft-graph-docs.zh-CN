---
title: eapFastConfiguration 枚举类型
description: EAP 快速配置的可用设置。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: db3f39eaeb375705c974e907ae4b0a177bd6c4ac
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526544"
---
# <a name="eapfastconfiguration-enum-type"></a>eapFastConfiguration 枚举类型

命名空间： microsoft. graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

EAP 快速配置的可用设置。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|noProtectedAccessCredential|0|使用 EAP-FAST （无保护性访问凭据（PAC））。|
|useProtectedAccessCredential|1 |使用受保护的访问凭据（PAC）。|
|useProtectedAccessCredentialAndProvision|2 |使用保护性接入身分凭证（PAC）和预配 PAC。|
|useProtectedAccessCredentialAndProvisionAnonymously|3 |使用受保护的访问凭据（PAC）、预配 PAC，并以匿名方式执行此操作。|



