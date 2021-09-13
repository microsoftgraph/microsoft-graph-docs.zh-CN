---
title: macOSFileVaultRecoveryKeyTypes 枚举类型
description: macOS FileVault 的恢复密钥类型
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c7f3d6fc43c38e2d5c51c909d64b0421230e876a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59106166"
---
# <a name="macosfilevaultrecoverykeytypes-enum-type"></a>macOSFileVaultRecoveryKeyTypes 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

macOS FileVault 的恢复密钥类型

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|设备默认值，无意图。|
|将coveryRecoveryKey|1|机构恢复密钥与"主"恢复密钥类似，可用于解锁密码丢失的任何设备。|
|personalRecoveryKey|2|个人恢复密钥是可用于解锁用户设备的唯一代码，即使设备密码丢失。|



