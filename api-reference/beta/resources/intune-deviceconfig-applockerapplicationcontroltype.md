---
title: appLockerApplicationControlType 枚举类型
description: AppLocker 应用程序控件类型的可能值
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b3bc89620a6dd13a65cfe40f37ba2f775e6a9c83
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425720"
---
# <a name="applockerapplicationcontroltype-enum-type"></a>appLockerApplicationControlType 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

AppLocker 应用程序控件类型的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|设备默认值，未选择的应用程序控制类型。|
|enforceComponentsAndStoreApps|1|强制实施 Windows 组件和 store 应用程序。|
|auditComponentsAndStoreApps|2|审核 Windows 组件和 store 应用程序。|
|enforceComponentsStoreAppsAndSmartlocker|3|强制实施 Windows 组件、 存储应用程序和智能锁定者。|
|auditComponentsStoreAppsAndSmartlocker|4|审核 Windows 组件，存储应用程序和智能锁定者。|




