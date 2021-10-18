---
title: appLockerApplicationControlType 枚举类型
description: AppLocker 应用程序控件类型的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: dbd02e9add1fe098c4f52762bc9aa8902633fc37
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60457314"
---
# <a name="applockerapplicationcontroltype-enum-type"></a>appLockerApplicationControlType 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

AppLocker 应用程序控件类型的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|设备默认值，未选择"应用程序控制"类型。|
|enforceComponentsAndStoreApps|1|强制Windows组件和存储应用。|
|auditComponentsAndStoreApps|2|审核Windows组件和存储应用。|
|enforceComponentsStoreAppsAndSmartlocker|3|强制Windows组件、应用商店应用和智能保险箱。|
|auditComponentsStoreAppsAndSmartlocker|4 |审核Windows组件、应用商店应用和智能保险箱。|



