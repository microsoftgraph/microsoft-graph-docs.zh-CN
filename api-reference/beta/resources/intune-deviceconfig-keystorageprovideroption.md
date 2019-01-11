---
title: keyStorageProviderOption 枚举类型
description: 密钥存储提供程序 (KSP) 导入选项。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4609092c3022b62331bbb6226a5b91e4b287ff79
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826465"
---
# <a name="keystorageprovideroption-enum-type"></a>keyStorageProviderOption 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

密钥存储提供程序 (KSP) 导入选项。
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|useTpmKspOtherwiseUseSoftwareKsp|0|导入到受信任平台模块 (TPM) KSP 如果存在此参数，否则导入到软件 KSP。|
|useTpmKspOtherwiseFail|1|导入到受信任平台模块 (TPM) KSP 如果存在此参数，否则会失败。|
|usePassportForWorkKspOtherwiseFail|2|导入到 Passport 工作 KSP 如果可用，否则失败。|
|useSoftwareKsp|3|导入到软件 KSP。|





