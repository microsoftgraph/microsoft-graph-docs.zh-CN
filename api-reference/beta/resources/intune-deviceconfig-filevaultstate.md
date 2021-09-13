---
title: fileVaultState 枚举类型
description: FileVault 状态
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1d9e037eb75fa331e082db5ca19e213c91a927c8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59075492"
---
# <a name="filevaultstate-enum-type"></a>fileVaultState 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

FileVault 状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|success|0|FileVault 状态成功|
|driveEncryptedByUser|1|FileVault 已由用户启用，并且未由策略管理|
|userDeferredEncryption|2|FileVault 策略已成功安装，但用户尚未开始加密|
|escrowNotEnabled|4 |未启用 FileVault 恢复密钥托管|



