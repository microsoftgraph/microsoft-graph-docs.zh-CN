---
title: educationSynchronizationCustomizations 资源类型
description: 包含要同步的实体列表及其自定义项（如果有）。
ms.localizationpriority: medium
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 30792f67b04606235a99e131d58ffb72bebe8ebd
ms.sourcegitcommit: 0ec845f93eaa140ad833ba163c76c5308197a92f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/01/2021
ms.locfileid: "60068585"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a>educationSynchronizationCustomizations 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含要同步的实体列表及其自定义项（如果有）。

> [!NOTE]
> 要同步的属性自定义不适用于学生注册或教师名单。

此资源是以下数据提供程序的成员：

- [educationCsvDataProvider](educationcsvdataprovider.md)
- [educationPowerSchoolDataProvider](educationpowerschooldataprovider.md)

## <a name="properties"></a>属性

| 属性          | 类型                                    | 说明                             |
| :---------------- | :-------------------------------------- | :-------------------------------------- |
| school            | [educationSynchronizationCustomization] | 学校实体的自定义。     |
| section           | [educationSynchronizationCustomization] | Section 实体的自定义项。    |
| student           | [educationSynchronizationCustomization] | 学生实体的自定义。    |
| teacher           | [educationSynchronizationCustomization] | 教师实体的自定义。    |
| studentEnrollment | [educationSynchronizationCustomization] | 学生注册的自定义。 |
| teacherRoster     | [educationSynchronizationCustomization] | 教师名单的自定义项。     |

[educationsynchronizationcustomization]: educationsynchronizationcustomization.md

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type&quot;: &quot;microsoft.graph.educationSynchronizationCustomizations"
}-->

```json
{
  "school": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization",
    "optionalPropertiesToSync": ["String"],
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate&quot;: &quot;Boolean"
  },
  "section": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization",
    "optionalPropertiesToSync": ["String"],
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate&quot;: &quot;Boolean"
  },
  "student": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization",
    "optionalPropertiesToSync": ["String"],
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate&quot;: &quot;Boolean"
  },
  "teacher": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization",
    "optionalPropertiesToSync": ["String"],
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate&quot;: &quot;Boolean"
  },
  "studentEnrollment": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization",
    "synchronizationStartDate": "DateTimeOffset",
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate&quot;: &quot;Boolean"
  },
  "teacherRoster": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomization",
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate&quot;: &quot;Boolean"
  }
}
```


