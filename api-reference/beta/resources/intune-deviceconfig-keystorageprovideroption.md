---
title: keyStorageProviderOption 枚举类型
description: 密钥存储提供程序 (KSP) 导入选项。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b422443abcdb72cd76399ae9f2e0fea59bb6f34f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460420"
---
# <a name="keystorageprovideroption-enum-type"></a>keyStorageProviderOption 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

密钥存储提供程序 (KSP) 导入选项。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|useTpmKspOtherwiseUseSoftwareKsp|0|导入到受信任的平台模块 (TPM) KSP (如果存在), 否则导入到软件 KSP。|
|useTpmKspOtherwiseFail|1|导入到受信任的平台模块 (TPM) KSP (如果存在), 否则会失败。|
|usePassportForWorkKspOtherwiseFail|2 |导入 Passport for work KSP (如果可用), 否则会失败。|
|useSoftwareKsp|3 |导入到软件 KSP。|





