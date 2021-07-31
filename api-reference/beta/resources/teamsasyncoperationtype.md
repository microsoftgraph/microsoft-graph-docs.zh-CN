---
title: teamsAsyncOperationType 枚举类型
description: teamsAsyncOperation 的类型。 由于支持更多异步操作，因此将在此处添加成员。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: enumPageType
ms.openlocfilehash: 8d29e2230dad68c4efbdb5b6bd51a39472de8680
ms.sourcegitcommit: 596b3d5636f3f3e042d180ea8f039f00ebd6b38a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2021
ms.locfileid: "53665807"
---
# <a name="teamsasyncoperationtype-enum-type"></a>teamsAsyncOperationType 枚举类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[teamsAsyncOperation 的类型](teamsasyncoperation.md)。 由于支持更多异步操作，因此将在此处添加成员。

## <a name="members"></a>成员
下表列出了可发展枚举 [的成员](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations)。 必须使用请求标头获取此可发展枚举中的以下 `Prefer: include-unknown-enum-members` 值 `teamifyGroup` `createChannel` `createChat` ：、、。

| 成员 | 说明 |
|:---------------|:----------|
|无效|值无效。|
|cloneTeam|克隆团队的操作。|
|archiveTeam|存档团队的操作。|
|unarchiveTeam|还原存档团队的操作。|
|createTeam|从头开始创建团队的操作。|
|unknownFutureValue| 可发展枚举 sentinel 值。 请勿使用。 |
|teamifyGroup |从组创建团队的操作。 |
|createChannel |在团队中创建频道的操作。 |
|createChat|从头开始创建聊天的操作。|
