---
title: vppTokenState 枚举类型
description: 与 Apple Volume Purchase Program 令牌关联的可能状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1789debbbc672d0ee195af788292fd556d25e899
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029328"
---
# <a name="vpptokenstate-enum-type"></a>vppTokenState 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

与 Apple Volume Purchase Program 令牌关联的可能状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|默认状态。|
|有效|1 |令牌有效。|
|期满|2 |令牌已过期。|
|无效|第三章|令牌无效。|
|assignedToExternalMDM|4 |令牌由另一个 MDM 服务管理。|
|duplicateLocationId|5 |令牌与帐户上的另一个令牌关联在同一位置。|






