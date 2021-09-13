---
title: windowsDefenderApplicationControlSupplementalPolicyStatuses 枚举类型
description: 各种 WindowsDefenderApplicationControl 补充策略部署状态的枚举值。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: fe8ed534f64188691f8e4cfd8e26322291f0f821
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59057192"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicystatuses-enum-type"></a>windowsDefenderApplicationControlSupplementalPolicyStatuses 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

各种 WindowsDefenderApplicationControl 补充策略部署状态的枚举值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|WindowsDefenderApplicationControl 补充策略的状态未知。|
|success|1|WindowsDefenderApplicationControl 补充策略有效。|
|tokenError|2|WindowsDefenderApplicationControl 补充策略在结构上可以正常使用，但授权令牌时出错。|
|notAuthorizedByToken|3|令牌不授权此 WindowsDefenderApplicationControl 补充策略。|
|policyNotFound|4 |未找到 WindowsDefenderApplicationControl 补充策略。|



