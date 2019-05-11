---
title: keyStorageProviderOption 枚举类型
description: 密钥存储提供程序 (KSP) 导入选项。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 77695c9deab823db79a3f8a98df16ff140d87248
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946264"
---
# <a name="keystorageprovideroption-enum-type"></a>keyStorageProviderOption 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

密钥存储提供程序 (KSP) 导入选项。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|useTpmKspOtherwiseUseSoftwareKsp|0|导入到受信任的平台模块 (TPM) KSP (如果存在), 否则导入到软件 KSP。|
|useTpmKspOtherwiseFail|1|导入到受信任的平台模块 (TPM) KSP (如果存在), 否则会失败。|
|usePassportForWorkKspOtherwiseFail|双面|导入 Passport for work KSP (如果可用), 否则会失败。|
|useSoftwareKsp|第三章|导入到软件 KSP。|




