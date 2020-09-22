---
title: teamsAsyncOperationStatus 枚举类型
description: 描述 teamsAsyncOperation 的当前状态。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ae88f15aa2f97a852d33074af8db85417ac3a66b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046511"
---
# <a name="teamsasyncoperationstatus-enum-type"></a>teamsAsyncOperationStatus 枚举类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述 [teamsAsyncOperation](teamsasyncoperation.md)的当前状态。

## <a name="members"></a>成员

| 成员 | 值| 说明 |
|:---------------|:--------|:----------|
|无效|0|值无效。|
|notStarted|1 |操作尚未开始。|
|inProgress|2 |操作正在运行。|
|完成|第三章|操作成功。|
|未能|4 |操作失败。|


