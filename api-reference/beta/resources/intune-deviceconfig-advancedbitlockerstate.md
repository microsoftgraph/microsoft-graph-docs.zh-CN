---
title: advancedBitLockerState 枚举类型
description: 高级 BitLocker 状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8ad93a61e03e923ef1c74121574ee5f4e9a94d36
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153597"
---
# <a name="advancedbitlockerstate-enum-type"></a>advancedBitLockerState 枚举类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

高级 BitLocker 状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|success|0|高级 BitLocker 状态成功|
|noUserConsent|1 |用户从未同意加密|
|osVolumeUnprotected|2 |检测到未受保护的操作系统卷|
|osVolumeTpmRequired|4 |TPM 不用于保护操作系统卷，但策略需要 TPM|
|osVolumeTpmOnlyRequired|8 |TPM 仅保护不用于操作系统卷，但策略需要|
|osVolumeTpmPinRequired|16 |TPM+PIN 保护不用于操作系统卷，但策略需要|
|osVolumeTpmStartupKeyRequired|32|TPM+启动密钥保护不用于操作系统卷，但策略需要|
|osVolumeTpmPinStartupKeyRequired|64|TPM+PIN+启动密钥不用于操作系统卷，但策略需要|
|osVolumeEncryptionMethodMismatch|128|操作系统卷的加密方法不同于策略设置的加密方法|
|recoveryKeyBackupFailed|256|恢复密钥备份失败|
|fixedDriveNotEncrypted|512|未加密的固定驱动器|
|fixedDriveEncryptionMethodMismatch|1024|固定驱动器的加密方法不同于策略设置的加密方法|
|loggedOnUserNonAdmin|2048|已登录的用户不是管理员。这需要将"AllowStandardUserEncryption"策略设置为 1|
|windowsRecoveryEnvironmentNotConfigured|4096|未配置 WinRE|
|tpmNotAvailable|8192|TPM 对 BitLocker 不可用。 这意味着 TPM 不存在，或者设置了 TPM 不可用的注册表覆盖或主机操作系统位于可移植/可移植的驱动器上|
|tpmNotReady|16384|TPM 未为 BitLocker 做好准备|
|networkError|32768|网络不可用。 恢复密钥备份需要这样做。 针对支持驱动器加密的设备报告这一点|




