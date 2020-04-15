---
title: appLockerApplicationControlType 枚举类型
description: AppLocker 应用程序控件类型的可能值
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a0f2509aff44de9ebd2c4ae5ea7db63bccfa604f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449138"
---
# <a name="applockerapplicationcontroltype-enum-type"></a>appLockerApplicationControlType 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

AppLocker 应用程序控件类型的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|设备默认值，未选择应用程序控件类型。|
|enforceComponentsAndStoreApps|1|强制实施 Windows 组件和应用商店应用。|
|auditComponentsAndStoreApps|双面|审核 Windows 组件和存储应用程序。|
|enforceComponentsStoreAppsAndSmartlocker|第三章|强制实施 Windows 组件、存储应用和智能保险箱。|
|auditComponentsStoreAppsAndSmartlocker|4 |审核 Windows 组件、存储应用和智能保险箱。|







