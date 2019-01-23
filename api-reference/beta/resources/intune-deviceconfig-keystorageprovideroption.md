---
title: keyStorageProviderOption 枚举类型
description: 密钥存储提供程序 (KSP) 导入选项。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6993d7e241ef94c572975c709c286a14f6eabf5b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424222"
---
# <a name="keystorageprovideroption-enum-type"></a>keyStorageProviderOption 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

密钥存储提供程序 (KSP) 导入选项。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|useTpmKspOtherwiseUseSoftwareKsp|0|导入到受信任平台模块 (TPM) KSP 如果存在此参数，否则导入到软件 KSP。|
|useTpmKspOtherwiseFail|1|导入到受信任平台模块 (TPM) KSP 如果存在此参数，否则会失败。|
|usePassportForWorkKspOtherwiseFail|2|导入到 Passport 工作 KSP 如果可用，否则失败。|
|useSoftwareKsp|3|导入到软件 KSP。|




