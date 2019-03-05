---
title: vppTokenState 枚举类型
description: 与 Apple volume Purchase Program 令牌关联的可能状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cdb356d5103fc1c1dc07245d8552cb77b9383c8b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159862"
---
# <a name="vpptokenstate-enum-type"></a>vppTokenState 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

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




