---
title: teamSpecialization 枚举类型
description: 描述为团队的特殊的使用情况。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c89f3ef993e55e28f5558f99c3ef87ad5174bc65
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640320"
---
# <a name="teamspecialization-enum-type"></a>teamSpecialization 枚举类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指示是否[团队](../resources/team.md)适用于特定用例。 每个[团队](../resources/team.md)具专业性有权访问唯一行为和针对其用例的体验。 默认值为无。

## <a name="members"></a>成员

| 成员             | 值 | 说明                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| 无               | 0     | 默认为团队通过该组件的标准团队体验的类型。          |
| educationStandard  | 1     | 培训用户创建的团队。 培训用户创建的所有团队都是类型 Edu。 |
| educationClass     | 2     | 团队优化类的体验。 这样跨 O365 细分的功能。 |
| educationProfessionalLearningCommunity | 3 | 针对 PLC 优化工作组体验。 了解有关 PLC[此处](https://en.wikipedia.org/wiki/Professional_learning_community)。 |
| educationStaff     | 4     |  为了优化的员工在组织中，员工主持人，如主体，其中是管理员，教师体验团队类型是附带专用笔记本团队中的成员。 有关详细信息，请参阅[面向教育机构的 OneNote 员工笔记本](https://www.onenote.com/staffnotebookedu)。 |
| unknownFutureValue | 7     | Sentinel 保留作为以供将来扩展枚举的占位符值。 |
<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error:{/api-reference/beta/resources/teamspecialization.md}:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
}-->
