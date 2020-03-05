---
title: teamsAsyncOperationStatus 枚举类型
description: 描述 teamsAsyncOperation 的当前状态。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2c82065c789847d3e2a11947dcf921b12c55530e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519895"
---
# <a name="teamsasyncoperationstatus-enum-type"></a>teamsAsyncOperationStatus 枚举类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述[teamsAsyncOperation](teamsasyncoperation.md)的当前状态。

## <a name="members"></a>成员

| 成员 | 值| 说明 |
|:---------------|:--------|:----------|
|无效|0|值无效。|
|notStarted|1 |操作尚未开始。|
|inProgress|2 |操作正在运行。|
|完成|3 |操作成功。|
|未能|4 |操作失败。|
