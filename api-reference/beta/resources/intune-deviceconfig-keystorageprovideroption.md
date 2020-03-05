---
title: keyStorageProviderOption 枚举类型
description: 密钥存储提供程序（KSP）导入选项。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8580688edbdacb150a37ee5cf2a52fdc77dd490f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526253"
---
# <a name="keystorageprovideroption-enum-type"></a>keyStorageProviderOption 枚举类型

命名空间： microsoft. graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

密钥存储提供程序（KSP）导入选项。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|useTpmKspOtherwiseUseSoftwareKsp|0|导入到受信任的平台模块（TPM） KSP （如果存在），否则导入到软件 KSP。|
|useTpmKspOtherwiseFail|1 |导入到受信任的平台模块（TPM） KSP （如果存在），否则会失败。|
|usePassportForWorkKspOtherwiseFail|2 |导入 Passport for work KSP （如果可用），否则会失败。|
|useSoftwareKsp|3 |导入到软件 KSP。|



