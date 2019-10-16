---
title: windowsDefenderApplicationControlSupplementalPolicyStatuses 枚举类型
description: 各种 WindowsDefenderApplicationControl 补充策略部署状态的枚举值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1999c999597d152396590e3faee6d7b472189500
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537655"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicystatuses-enum-type"></a>windowsDefenderApplicationControlSupplementalPolicyStatuses 枚举类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

各种 WindowsDefenderApplicationControl 补充策略部署状态的枚举值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|WindowsDefenderApplicationControl 补充策略的状态未知。|
|success|1|WindowsDefenderApplicationControl 补充策略生效。|
|tokenError|双面|WindowsDefenderApplicationControl 补充策略在结构上是正常的，但在授权令牌时发生错误。|
|notAuthorizedByToken|第三章|令牌不授权此 WindowsDefenderApplicationControl 补充策略。|
|policyNotFound|4 |找不到 WindowsDefenderApplicationControl 补充策略。|



