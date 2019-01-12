---
title: vppTokenState 枚举类型
description: 使用 Apple 卷购买计划令牌关联可能的状态。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6bdeb73b6491f3960ce30db91a35d06c0f8ffaf1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986661"
---
# <a name="vpptokenstate-enum-type"></a>vppTokenState 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

使用 Apple 卷购买计划令牌关联可能的状态。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|默认状态。|
|有效|1|令牌有效。|
|过期|2|令牌已过期。|
|无效|3|令牌无效。|
|assignedToExternalMDM|4|由另一个 MDM 服务管理令牌。|



