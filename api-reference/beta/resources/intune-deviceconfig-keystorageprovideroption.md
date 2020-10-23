---
title: keyStorageProviderOption 枚举类型
description: 密钥存储提供程序 (KSP) 导入选项。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 2c97c592f7e7f3a3d2a154d24dc4c331ba62c5b1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697929"
---
# <a name="keystorageprovideroption-enum-type"></a>keyStorageProviderOption 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

密钥存储提供程序 (KSP) 导入选项。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|useTpmKspOtherwiseUseSoftwareKsp|0|导入到受信任的平台模块 (TPM) KSP （如果存在），否则导入到软件 KSP。|
|useTpmKspOtherwiseFail|1|导入到受信任的平台模块 (TPM) KSP （如果存在），否则会失败。|
|usePassportForWorkKspOtherwiseFail|双面|导入 Passport for work KSP （如果可用），否则会失败。|
|useSoftwareKsp|第三章|导入到软件 KSP。|





