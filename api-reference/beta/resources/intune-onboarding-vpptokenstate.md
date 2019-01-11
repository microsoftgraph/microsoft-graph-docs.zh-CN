---
title: vppTokenState 枚举类型
description: 使用 Apple 卷购买计划令牌关联可能的状态。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b91090f64340e398bf9d48aff3741941fc0d778a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844833"
---
# <a name="vpptokenstate-enum-type"></a>vppTokenState 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

使用 Apple 卷购买计划令牌关联可能的状态。
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|unknown|0|默认状态。|
|有效|1|令牌有效。|
|过期|2|令牌已过期。|
|无效|3|令牌无效。|
|assignedToExternalMDM|4|由另一个 MDM 服务管理令牌。|





