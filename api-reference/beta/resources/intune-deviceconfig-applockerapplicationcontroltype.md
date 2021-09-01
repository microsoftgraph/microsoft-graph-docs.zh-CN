---
title: appLockerApplicationControlType 枚举类型
description: AppLocker 应用程序控件类型的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 617db7bd086ff14611804c12506cc58b5a446d10
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58791907"
---
# <a name="applockerapplicationcontroltype-enum-type"></a>appLockerApplicationControlType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

AppLocker 应用程序控件类型的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|设备默认值，未选择"应用程序控制"类型。|
|enforceComponentsAndStoreApps|1|强制Windows组件和存储应用。|
|auditComponentsAndStoreApps|2|审核Windows组件和存储应用。|
|enforceComponentsStoreAppsAndSmartlocker|3|强制Windows组件、存储应用和智能保险箱。|
|auditComponentsStoreAppsAndSmartlocker|4 |审核Windows组件、应用商店应用和智能保险箱。|



