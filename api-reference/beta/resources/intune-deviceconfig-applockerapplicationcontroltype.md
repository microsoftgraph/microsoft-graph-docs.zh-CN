---
title: appLockerApplicationControlType 枚举类型
description: AppLocker 应用程序控件类型的可能值
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a1b3e5ec545f4466eb080f20839e12c7e5972cc0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34981578"
---
# <a name="applockerapplicationcontroltype-enum-type"></a>appLockerApplicationControlType 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

AppLocker 应用程序控件类型的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|设备默认值, 未选择应用程序控件类型。|
|enforceComponentsAndStoreApps|1|强制实施 Windows 组件和应用商店应用。|
|auditComponentsAndStoreApps|双面|审核 Windows 组件和存储应用程序。|
|enforceComponentsStoreAppsAndSmartlocker|第三章|强制实施 Windows 组件、存储应用和智能保险箱。|
|auditComponentsStoreAppsAndSmartlocker|4|审核 Windows 组件、存储应用和智能保险箱。|





