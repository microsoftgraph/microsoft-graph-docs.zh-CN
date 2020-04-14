---
title: windowsPrivacyDataAccessLevel 枚举类型
description: 确定特定 Windows 隐私数据类别的访问级别。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: deebb9f7d24646d18b425b0948eb4a229341fb6d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444055"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a>windowsPrivacyDataAccessLevel 枚举类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

确定特定 Windows 隐私数据类别的访问级别。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|未指定访问级别，无意向。 在 UserInControl 或 ForceAllow 中，设备的行为可能是一样的。 它可能取决于访问的隐私数据、Windows 版本和其他因素。|
|forceAllow|1|将允许应用访问指定的隐私数据。|
|forceDeny|双面|将拒绝应用程序访问指定的隐私数据。|
|userInControl|第三章|当应用尝试访问指定的隐私数据时，系统将提示用户。|



