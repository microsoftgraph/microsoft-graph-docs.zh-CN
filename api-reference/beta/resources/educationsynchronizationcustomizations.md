---
title: educationSynchronizationCustomizations 资源类型
description: 如果有，包含与同步和其自定义的实体列表。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 3254915887afc1e6b0da0b3b6c44b59689219ab1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918187"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a>educationSynchronizationCustomizations 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

如果有，包含同步和其[自定义项](educationsynchronizationcustomization.md)的实体列表。

> **注意：** 要同步的属性的自定义不适用于**studentEnrollment**和**teacherRoster**实体。

此资源是以下数据提供程序的成员：

* [educationCsvDataProvider](educationcsvdataprovider.md)
* [educationPowerSchoolDataProvider](educationpowerschooldataprovider.md)

## <a name="properties"></a>属性

| 属性 | 类型 | Description |
|:-|:-|:-|
| **学校** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  学校实体的自定义。        |
| **section** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  针对部分实体的自定义项。         |
| **student** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  学生实体的自定义。         |
| **teacher** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  教师实体的自定义。         |
| **studentEnrollment** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |  针对学生注册自定义项。           |
| **teacherRoster** | [educationSynchronizationCustomization](educationsynchronizationcustomization.md) |       针对教师名单的自定义项。    |

## <a name="json-representation"></a>JSON 表示形式
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationCustomizations"
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
