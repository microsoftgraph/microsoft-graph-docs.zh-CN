---
title: keyStorageProviderOption 枚举类型
description: 密钥存储提供程序 (KSP) 导入选项。
ms.openlocfilehash: 236489d288ec0be70a818e1c51b8c634ad3933a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042374"
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





