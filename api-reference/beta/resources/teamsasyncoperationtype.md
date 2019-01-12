---
title: teamsAsyncOperationType 枚举类型
description: TeamsAsyncOperation 的类型。 将要添加的成员此处为多个异步支持操作。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1770f642970575647dd1216038202fca15f82117
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987305"
---
# <a name="teamsasyncoperationtype-enum-type"></a>teamsAsyncOperationType 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

[TeamsAsyncOperation](teamsasyncoperation.md)的类型。 将要添加的成员此处为多个异步支持操作。

## <a name="members"></a>成员

| 成员 | 值| 说明 |
|:---------------|:--------|:----------|
|无效|0|值无效。|
|cloneTeam|1|要克隆团队的操作。|
|archiveTeam|2|若要存档团队的操作。|
|unarchiveTeam|3|若要还原的存档的团队的操作。|
|createTeam|3|若要从头开始创建团队的操作。|

