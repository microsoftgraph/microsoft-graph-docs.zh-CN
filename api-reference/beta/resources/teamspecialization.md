---
title: teamSpecialization 枚举类型
description: 描述为团队的特殊的使用情况。
ms.openlocfilehash: 8f50e158e6eedc964226478841c5322eefca9f77
ms.sourcegitcommit: 12c6e82f1417022540e534ebadbd0e8d7fb5abde
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2018
ms.locfileid: "27210136"
---
# <a name="teamspecialization-enum-type"></a>teamSpecialization 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

指示是否[团队](../resources/team.md)适用于特定用例。 每个[团队](../resources/team.md)具专业性有权访问唯一行为和针对其用例的体验。 默认值为无。

## <a name="members"></a>成员

| 成员             | 值 | 说明                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| 无               | 0     | 默认为团队通过该组件的标准团队体验的类型。          |
| unknownFutureValue | 7     | Sentinel 保留作为以供将来扩展枚举的占位符值。 |
