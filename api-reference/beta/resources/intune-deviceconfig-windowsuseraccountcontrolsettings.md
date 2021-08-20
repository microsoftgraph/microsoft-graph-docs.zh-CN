---
title: windowsUserAccountControlSettings 枚举类型
description: 用户帐户控制Windows的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: dcbc9fb708aeec862bc9de3b070ffd4ca527171f90f9740e1356e2a1ef615035
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54206478"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a>windowsUserAccountControlSettings 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户帐户控制Windows的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|userDefined|0|用户定义，默认值，无意图。|
|alwaysNotify|1 |始终通知。|
|notifyOnAppChanges|2 |通知应用更改。|
|notifyOnAppChangesWithoutDimming|3 |通知应用更改时，桌面不会变暗。|
|neverNotify|4 |从不通知。|




