---
title: teamsAsyncOperationType 枚举类型
description: teamsAsyncOperation 的类型。 由于支持更多异步操作，因此将在此处添加成员。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: enumPageType
ms.openlocfilehash: 5765fabd5e9b13f040c6f7b189a31223414fc0a0
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030829"
---
# <a name="teamsasyncoperationtype-enum-type"></a>teamsAsyncOperationType 枚举类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[teamsAsyncOperation 的类型](teamsasyncoperation.md)。 由于支持更多异步操作，因此将在此处添加成员。

## <a name="members"></a>成员

| 成员 | 值| 说明 |
|:---------------|:--------|:----------|
|无效|0|值无效。|
|cloneTeam|1|克隆团队的操作。|
|archiveTeam|2|存档团队的操作。|
|unarchiveTeam|3|还原存档团队的操作。|
|createTeam|4 |从头开始创建团队的操作。|
|createChat|5 |从头开始创建聊天的操作。|
