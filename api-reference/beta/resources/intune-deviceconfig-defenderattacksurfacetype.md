---
title: defenderAttackSurfaceType 枚举类型
description: Defender 攻击面减少规则的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 435ce477f60f14437a05e22fd5c670cbe1b25796
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256650"
---
# <a name="defenderattacksurfacetype-enum-type"></a>defenderAttackSurfaceType 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Defender 攻击面减少规则的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|定制|0|默认值，它禁用攻击面降低规则。|
|数据|1|启用攻击面降低规则。|
|auditMode|双面|如果启用，请评估 ASR 规则将如何影响你的组织。 不会更改功能，而是生成日志。|
|警告|6 |向最终用户发出的警告消息，能够绕过受攻击面降低规则阻止的阻止。|
|disable|99|禁用攻击面降低规则|




