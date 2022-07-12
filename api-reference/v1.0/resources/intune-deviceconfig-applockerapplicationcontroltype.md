---
title: appLockerApplicationControlType 枚举类型
description: AppLocker 应用程序控件类型的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 94c6bb7c68bb97afa769de05f872875638f4bd8f
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730719"
---
# <a name="applockerapplicationcontroltype-enum-type"></a>appLockerApplicationControlType 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

AppLocker 应用程序控件类型的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|设备默认值，未选择应用程序控制类型。|
|enforceComponentsAndStoreApps|1|强制实施 Windows 组件和应用商店应用。|
|auditComponentsAndStoreApps|2|审核 Windows 组件和应用商店应用。|
|enforceComponentsStoreAppsAndSmartlocker|3|强制实施 Windows 组件、应用商店和智能储物柜。|
|auditComponentsStoreAppsAndSmartlocker|4|审核 Windows 组件、应用商店和智能储物柜。|





