---
title: teamSpecialization 枚举类型
description: 描述为团队的特殊的使用情况。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 02a2272ee085d0c265adc9ce2e3f1c598e45be21
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930283"
---
# <a name="teamspecialization-enum-type"></a>teamSpecialization 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

指示是否[团队](../resources/team.md)适用于特定用例。 每个[团队](../resources/team.md)具专业性有权访问唯一行为和针对其用例的体验。 默认值为无。

## <a name="members"></a>成员

| 成员             | 值 | Description                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| 无               | 0     | 默认为团队通过该组件的标准团队体验的类型。          |
| unknownFutureValue | 7     | Sentinel 保留作为以供将来扩展枚举的占位符值。 |
