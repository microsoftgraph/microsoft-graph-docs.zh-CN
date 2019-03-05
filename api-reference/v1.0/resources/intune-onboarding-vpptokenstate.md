---
title: vppTokenState 枚举类型
description: 与 Apple volume Purchase Program 令牌关联的可能状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 573fe27064881f670e642e7c3727b8c9eb7db5a9
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254931"
---
# <a name="vpptokenstate-enum-type"></a>vppTokenState 枚举类型

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

与 Apple volume Purchase Program 令牌关联的可能状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|默认状态。|
|有效|1|令牌有效。|
|期满|双面|令牌已过期。|
|无效|第三章|令牌无效。|
|assignedToExternalMDM|4|令牌由另一个 MDM 服务管理。|



