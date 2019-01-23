---
title: windowsUserAccountControlSettings 枚举类型
description: 对于 Windows 用户帐户控制设置的可能值。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ff348fd33e6bbc8370378783cf0a517a205ea101
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399813"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a>windowsUserAccountControlSettings 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

对于 Windows 用户帐户控制设置的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|用户定制|0|用户定义，默认值、 没有用途。|
|alwaysNotify|1|始终通知。|
|notifyOnAppChanges|2|通知应用程序的更改。|
|notifyOnAppChangesWithoutDimming|3|不变暗桌面通知应用程序的更改。|
|neverNotify|4|从不通知。|




