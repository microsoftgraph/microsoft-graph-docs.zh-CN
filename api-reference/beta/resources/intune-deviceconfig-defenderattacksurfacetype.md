---
title: defenderAttackSurfaceType 枚举类型
description: Defender 攻击面减少规则的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 244523298e0d548763a0ce61aaa09478ae6b9111
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58797920"
---
# <a name="defenderattacksurfacetype-enum-type"></a>defenderAttackSurfaceType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Defender 攻击面减少规则的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|userDefined|0|默认值，禁用攻击面减少规则。|
|block|1|启用攻击面减少规则。|
|auditMode|2|评估 ASR 规则在启用后对组织的影响。 不更改功能，但生成日志。|
|warn|6 |向能够绕过攻击面减少规则阻止的最终用户发送的警告消息。|
|disable|99|禁用攻击面减少规则|



