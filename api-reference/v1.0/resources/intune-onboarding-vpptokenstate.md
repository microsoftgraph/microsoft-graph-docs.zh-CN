---
title: vppTokenState 枚举类型
description: 与 Apple Volume Purchase Program 令牌关联的可能状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 644b1d58a38d23d71a2fa56e7bfd5d678ffee76e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447995"
---
# <a name="vpptokenstate-enum-type"></a>vppTokenState 枚举类型

命名空间： microsoft. graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

与 Apple Volume Purchase Program 令牌关联的可能状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|默认状态。|
|有效|1 |令牌有效。|
|期满|2 |令牌已过期。|
|无效|3 |令牌无效。|
|assignedToExternalMDM|4 |令牌由另一个 MDM 服务管理。|




