---
title: fileVaultState 枚举类型
description: FileVault 状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4d2e038d5f75f25bb534bfc5923b946d0a0dfd16
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994139"
---
# <a name="filevaultstate-enum-type"></a>fileVaultState 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

FileVault 状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|success|0|FileVault 状态成功|
|driveEncryptedByUser|1 |FileVault 已由用户启用，且不受策略管理|
|userDeferredEncryption|2 |FileVault 策略已成功安装，但用户尚未开始加密|
|escrowNotEnabled|4 |FileVault 未启用恢复密钥的保管功能|






