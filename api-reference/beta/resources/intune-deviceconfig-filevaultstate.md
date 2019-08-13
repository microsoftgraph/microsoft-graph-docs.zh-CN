---
title: fileVaultState 枚举类型
description: FileVault 状态
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 54e8076dc4b4f6ab20f7790d2a650de6c07aa702
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325566"
---
# <a name="filevaultstate-enum-type"></a>fileVaultState 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

FileVault 状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|success|0|FileVault 状态成功|
|driveEncryptedByUser|1|FileVault 已由用户启用, 且不受策略管理|
|userDeferredEncryption|双面|FileVault 策略已成功安装, 但用户尚未开始加密|
|escrowNotEnabled|4|FileVault 未启用恢复密钥的保管功能|



