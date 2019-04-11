---
title: windowsPrivacyDataAccessLevel 枚举类型
description: 确定特定 Windows 隐私数据类别的访问级别。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 10486899094cf275cb3fb9254114d92cb7d12388
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31788105"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a>windowsPrivacyDataAccessLevel 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

确定特定 Windows 隐私数据类别的访问级别。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|未指定访问级别, 无意向。 在 UserInControl 或 ForceAllow 中, 设备的行为可能是一样的。 它可能取决于访问的隐私数据、Windows 版本和其他因素。|
|forceAllow|1|将允许应用访问指定的隐私数据。|
|forceDeny|双面|将拒绝应用程序访问指定的隐私数据。|
|userInControl|第三章|当应用尝试访问指定的隐私数据时, 系统将提示用户。|





