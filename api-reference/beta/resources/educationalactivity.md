---
title: educationalActivity 资源类型
description: educationalActivity 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 8d060de55d765adb7e01e6b03842c569f03c8d4f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939619"
---
# <a name="educationalactivity-resource-type"></a>educationalActivity 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用户已提供与 undergraduate、毕业、postgraduate 或其他教学活动相关的数据。

继承[itemFacet](itemfacet.md)中的元数据属性。

## <a name="methods"></a>方法

| 方法                                                       | 返回类型                                   | 说明                                                      |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [获取 educationalActivity](../api/educationalactivity-get.md) | [educationalActivity](educationalactivity.md) | 读取 educationalActivity 对象的属性和关系。 |
| [Update](../api/educationalactivity-update.md)               | [educationalActivity](educationalactivity.md) | 更新 educationalActivity 对象。                               |
| [删除](../api/educationalactivity-delete.md)               | 无                                          | 删除 educationalActivity 对象。                               |

## <a name="properties"></a>属性

| 属性           | 类型                                                      | 描述                                                                |
|:-------------------|:----------------------------------------------------------|:---------------------------------------------------------------------------|
|completionMonthYear |日期                                                       |用户逐步或完成活动的月份和年份。            |
|endMonthYear        |日期                                                       |用户完成所引用的教育活动的月份和年份。  |
|机构         |[institutionData](institutiondata.md)                      |包含在上研究的机构的详细信息。                             |
|主程序             |[educationalActivityDetail](educationalactivitydetail.md)  |包含有关程序或课程的扩展信息。                  |
|startMonthYear      |日期                                                       |用户 commenced 引用的活动的月份和年份。              |

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationalActivity",
  "baseType": ""
}-->

```json
{
  "completionMonthYear": "String (timestamp)",
  "endMonthYear": "String (timestamp)",
  "institution": {"@odata.type": "microsoft.graph.institutionData"},
  "program": {"@odata.type": "microsoft.graph.educationalActivityDetail"},
  "startMonthYear": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationalActivity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->