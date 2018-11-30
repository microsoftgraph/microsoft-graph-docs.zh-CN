---
title: appLockerApplicationControlType 枚举类型
description: AppLocker 应用程序控件类型的可能值
ms.openlocfilehash: 150e3daa6b8deb2d1e17c3ea7caf345ba39446f3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043891"
---
# <a name="applockerapplicationcontroltype-enum-type"></a>appLockerApplicationControlType 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

AppLocker 应用程序控件类型的可能值
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|设备默认值，未选择的应用程序控制类型。|
|enforceComponentsAndStoreApps|1|强制实施 Windows 组件和 store 应用程序。|
|auditComponentsAndStoreApps|2|审核 Windows 组件和 store 应用程序。|
|enforceComponentsStoreAppsAndSmartlocker|3|强制实施 Windows 组件、 存储应用程序和智能锁定者。|
|auditComponentsStoreAppsAndSmartlocker|4|审核 Windows 组件，存储应用程序和智能锁定者。|





