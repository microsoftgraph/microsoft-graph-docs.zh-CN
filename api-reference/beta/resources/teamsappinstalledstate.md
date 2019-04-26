---
title: Members
description: 描述 teamsApp 的当前安装状态。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 51be91c5ef09845c53c6eb1388c1fd5b68333b21
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341622"
---
#<a name="teamsappinstalledstate-enum-type"></a>teamsAppInstalledState 枚举类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述[teamsApp](teamsapp.md)的当前安装状态。

## <a name="members"></a>成员

| 成员 | 值| 说明 |
|:---------------|:--------|:----------|
|notInstalled|0|未将应用安装到团队。|
|了|1|应用程序以正常方式安装。|
|installedAndHidden|双面|已安装应用程序, 但已在视图中隐藏。|
|installedAndPermanent|第三章|应用程序永久安装且不可能删除。|
