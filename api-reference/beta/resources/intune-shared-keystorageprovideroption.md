---
title: keyStorageProviderOption 枚举类型
description: Key 存储 Provider (KSP) Import Options.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9f8f47384333189f80d6443a17027e62b1a1e465
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59030002"
---
# <a name="keystorageprovideroption-enum-type"></a>keyStorageProviderOption 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Key 存储 Provider (KSP) Import Options.

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|useTpmKspOtherwiseUseSoftwareKsp|0|导入到受信任平台模块 (TPM) KSP（如果存在）中，否则导入到软件 KSP。|
|useTpmKspOtherwiseFail|1|导入到受信任平台模块 (TPM) KSP（如果存在）否则会失败。|
|usePassportForWorkKspOtherwiseFail|2|如果可用，请导入到 Passport 中工作 KSP，否则会失败。|
|useSoftwareKsp|3|导入到软件 KSP。|



