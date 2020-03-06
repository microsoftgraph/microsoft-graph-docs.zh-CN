---
title: appLockerApplicationControlType 枚举类型
description: AppLocker 应用程序控件类型的可能值
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ca428eb0ccf9121cc3a7b02e6abb333e0b4e5503
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530925"
---
# <a name="applockerapplicationcontroltype-enum-type"></a>appLockerApplicationControlType 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

AppLocker 应用程序控件类型的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|设备默认值，未选择应用程序控件类型。|
|enforceComponentsAndStoreApps|1 |强制实施 Windows 组件和应用商店应用。|
|auditComponentsAndStoreApps|2 |审核 Windows 组件和存储应用程序。|
|enforceComponentsStoreAppsAndSmartlocker|3 |强制实施 Windows 组件、存储应用和智能保险箱。|
|auditComponentsStoreAppsAndSmartlocker|4 |审核 Windows 组件、存储应用和智能保险箱。|




