---
title: educationSynchronizationCustomizations 资源类型
description: 包含要同步的实体的列表及其自定义项 (如果有)。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 0d1a886557e37bb19b23c5e0c1d74b937112cc58
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334102"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a>educationSynchronizationCustomizations 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含要同步的实体的列表及其[自定义项](educationsynchronizationcustomization.md)(如果有)。

> **注意:** 要同步的属性的自定义不应用于**studentEnrollment**和**teacherRoster**实体。

此资源是以下数据提供程序的成员:

* [educationCsvDataProvider](educationcsvdataprovider.md)
* [educationPowerSchoolDataProvider](educationpowerschooldataprovider.md)

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-|:-|:-|
| **虽然** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  自定义的学校实体。        |
| **section** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  节实体的自定义项。         |
| **student** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  学生实体的自定义。         |
| **teacher** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  为教师实体自定义。         |
| **studentEnrollment** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  学生注册的自定义。           |
| **teacherRoster** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |       教师名单的自定义。    |

## <a name="json-representation"></a>JSON 表示形式
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
}-->

```json
{
  "school": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "section": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "student": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "teacher": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "studentEnrollment": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "teacherRoster": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"}
}
```
