---
title: keyStorageProviderOption 枚举类型
description: Key 存储 Provider (KSP) Import Options.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7bfd89c8e74264aca79af72325d6b5b4a96b23a3a3fadd44b32c94f3fa95cc58
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54219750"
---
# <a name="keystorageprovideroption-enum-type"></a>keyStorageProviderOption 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Key 存储 Provider (KSP) Import Options.

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|useTpmKspOtherwiseUseSoftwareKsp|0|导入到受信任平台模块 (TPM) ，如果存在，则导入到软件 KSP。|
|useTpmKspOtherwiseFail|1 |导入到受信任平台模块 (TPM) KSP（如果存在）否则会失败。|
|usePassportForWorkKspOtherwiseFail|2 |如果可用，请导入到 Passport 中工作 KSP，否则会失败。|
|useSoftwareKsp|3 |导入到软件 KSP。|




