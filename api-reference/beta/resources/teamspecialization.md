---
title: teamSpecialization 枚举类型
description: 描述团队的特殊用例。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8700896c32a83a3e157186f405c435589ce03815
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345679"
---
# <a name="teamspecialization-enum-type"></a>teamSpecialization 枚举类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指示[团队](../resources/team.md)是否适用于特定用例。 每个[团队](../resources/team.md)特殊化都有权访问针对其用例的独特行为和体验。 默认值为 "无"。

## <a name="members"></a>成员

| 成员             | 值 | 说明                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| 无               | 0     | 团队的默认类型, 可提供标准团队体验。          |
| educationStandard  | 1     | 由教育用户创建的团队。 教育用户创建的所有团队都属于 Edu 类型。 |
| educationClass     | 双面     | 针对某个类进行了优化的团队体验。 这样可以跨 O365 分段功能。 |
| educationProfessionalLearningCommunity | 第三章 | 为 PLC 优化的团队体验。 [在此处](https://en.wikipedia.org/wiki/Professional_learning_community)了解有关 PLC 的详细信息。 |
| educationStaff     | 4     |  对于组织中员工的优化体验的团队类型, 员工主管 (如主体) 是管理员, 而教师是一个专门的笔记本提供的团队成员。 有关更多详细信息, 请参阅[OneNote 教职员工笔记本教育](https://www.onenote.com/staffnotebookedu)版。 |
| 向 unknownfuturevalue | 步     | 将 Sentinel 值保留为占位符, 以便将来扩展枚举。 |
