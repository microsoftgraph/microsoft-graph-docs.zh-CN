---
title: teamsAsyncOperationStatus 枚举类型
description: 介绍 teamsAsyncOperation 的当前状态。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: b6af5c7218a6a9d8c0c5338beb8cdf9944a56c2e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858973"
---
# <a name="teamsasyncoperationstatus-enum-type"></a>teamsAsyncOperationStatus 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

介绍[teamsAsyncOperation](teamsasyncoperation.md)的当前状态。

## <a name="members"></a>成员

| 成员 | 值| Description |
|:---------------|:--------|:----------|
|无效|0|值无效。|
|为 notStarted|1|尚未开始此操作。|
|正在进行|2|正在运行的操作。|
|succeeded|3|操作成功。|
|failed|4|操作失败。|
