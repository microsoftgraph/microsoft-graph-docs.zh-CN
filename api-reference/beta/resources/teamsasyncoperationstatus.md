---
title: teamsAsyncOperationStatus 枚举类型
description: 介绍 teamsAsyncOperation 的当前状态。
ms.openlocfilehash: f553242ace983651b8d4fda77370de712f9d08b6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042429"
---
# <a name="teamsasyncoperationstatus-enum-type"></a>teamsAsyncOperationStatus 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

介绍[teamsAsyncOperation](teamsasyncoperation.md)的当前状态。

## <a name="members"></a>成员

| 成员 | 值| 说明 |
|:---------------|:--------|:----------|
|无效|0|值无效。|
|为 notStarted|1|尚未开始此操作。|
|正在进行|2|正在运行的操作。|
|succeeded|3|操作成功。|
|failed|4|操作失败。|