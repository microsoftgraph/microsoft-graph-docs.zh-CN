---
title: educationSynchronizationCustomizations 资源类型
description: 包含要同步的实体的列表及其自定义项（如果有）。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d3bfbec774b0ce5ff749e78b0057799501f432c3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055588"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a>educationSynchronizationCustomizations 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含要同步的实体的列表及其自定义项（如果有）。

> [!NOTE]
> 要同步的属性的自定义不适用于学生注册或教师名册。

此资源是以下数据提供程序的成员：

- [educationCsvDataProvider](educationcsvdataprovider.md)
- [educationPowerSchoolDataProvider](educationpowerschooldataprovider.md)

## <a name="properties"></a>属性

| 属性          | 类型                                    | 说明                             |
| :---------------- | :-------------------------------------- | :-------------------------------------- |
| 虽然            | [educationSynchronizationCustomization] | 学校实体的自定义项。     |
| section           | [educationSynchronizationCustomization] | 节实体的自定义项。    |
| student           | [educationSynchronizationCustomization] | 学生实体的自定义项。    |
| teacher           | [educationSynchronizationCustomization] | 教师实体的自定义项。    |
| studentEnrollment | [educationSynchronizationCustomization] | 学生登记的自定义项。 |
| teacherRoster     | [educationSynchronizationCustomization] | 教师名册的自定义项。     |

[educationsynchronizationcustomization]: educationsynchronizationcustomization.md

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
}-->

```json
{
  "school": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  },
  "section": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  },
  "student": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  },
  "teacher": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  },
  "studentEnrollment": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  },
  "teacherRoster": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
  }
}
```


