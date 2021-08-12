---
title: vppTokenState 枚举类型
description: 与 Apple Volume Purchase Program 令牌关联的可能状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 6f83fb497c5c331d8662853bff58bbca36b14c35dadbfb9f89f5feddbe032ed4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141551"
---
# <a name="vpptokenstate-enum-type"></a>vppTokenState 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

与 Apple Volume Purchase Program 令牌关联的可能状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|默认状态。|
|valid|1|令牌有效。|
|已过期|2|令牌已过期。|
|无效|3|令牌无效。|
|assignedToExternalMDM|4 |令牌由另一个 MDM 服务管理。|




