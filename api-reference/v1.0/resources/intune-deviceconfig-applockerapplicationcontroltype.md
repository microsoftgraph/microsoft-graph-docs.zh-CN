---
title: appLockerApplicationControlType 枚举类型
description: AppLocker 应用程序控件类型的可能值
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 241387f34a64b4b58d974fc21e2aa5d3af696736
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871979"
---
# <a name="applockerapplicationcontroltype-enum-type"></a>appLockerApplicationControlType 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

AppLocker 应用程序控件类型的可能值
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|notConfigured|0|设备默认值，未选择的应用程序控制类型。|
|enforceComponentsAndStoreApps|1|强制实施 Windows 组件和 store 应用程序。|
|auditComponentsAndStoreApps|2|审核 Windows 组件和 store 应用程序。|
|enforceComponentsStoreAppsAndSmartlocker|3|强制实施 Windows 组件、 存储应用程序和智能锁定者。|
|auditComponentsStoreAppsAndSmartlocker|4|审核 Windows 组件，存储应用程序和智能锁定者。|



