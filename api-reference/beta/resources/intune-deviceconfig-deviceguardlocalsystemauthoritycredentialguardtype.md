---
title: deviceGuardLocalSystemAuthorityCredentialGuardType 枚举类型
description: Credential Guard 设置的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c4369a5bf5752edf9c0636f31f936ecd43048407
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58817108"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a>deviceGuardLocalSystemAuthorityCredentialGuardType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Credential Guard 设置的可能值。

## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|notConfigured|0|如果之前未配置 UEFI 锁定，则远程关闭 Credential Guard。|
|enableWithUEFILock|1|使用 UEFI 锁定打开 Credential Guard。|
|enableWithoutUEFILock|2|在没有 UEFI 锁定的情况下打开 Credential Guard。|
|disable|3|禁用 Credential Guard。 这是默认的操作系统值。|



