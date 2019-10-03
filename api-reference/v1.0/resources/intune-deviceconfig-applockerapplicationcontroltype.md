---
title: appLockerApplicationControlType 枚举类型
description: AppLocker 应用程序控件类型的可能值
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e54aeb4658177531677d875c8b72413f3e4c1ee4
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366704"
---
# <a name="applockerapplicationcontroltype-enum-type"></a>appLockerApplicationControlType 枚举类型

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

AppLocker 应用程序控件类型的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|设备默认值，未选择应用程序控件类型。|
|enforceComponentsAndStoreApps|1|强制实施 Windows 组件和应用商店应用。|
|auditComponentsAndStoreApps|双面|审核 Windows 组件和存储应用程序。|
|enforceComponentsStoreAppsAndSmartlocker|第三章|强制实施 Windows 组件、存储应用和智能保险箱。|
|auditComponentsStoreAppsAndSmartlocker|4|审核 Windows 组件、存储应用和智能保险箱。|




