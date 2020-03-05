---
title: workPosition 资源类型
description: workPosition 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 086273e54d923054ce8e71ef1c67fb2bb4f7002a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519062"
---
# <a name="workposition-resource-type"></a>workPosition 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关与用户[配置文件](profile.md)相关联的工作职位的详细信息。

此资源类型继承自[itemFacet](itemfacet.md)。

## <a name="methods"></a>方法

| 方法                                         | 返回类型                     | 说明                                               |
|:-----------------------------------------------|:--------------------------------|:----------------------------------------------------------|
| [获取 workPosition](../api/workposition-get.md) | [workPosition](workposition.md) | 读取**workPosition**对象的属性和关系。 |
| [更新 workPosition](../api/workposition-update.md)        | [workPosition](workposition.md) | 更新**workPosition**对象。                               |
| [删除 workPosition](../api/workposition-delete.md)        | 无                            | 删除**workPosition**对象。                               |

## <a name="properties"></a>属性

| 属性             | 类型                               | 说明                                                                                                |
|:---------------------|:-----------------------------------|:-----------------------------------------------------------------------------------------------------------|
|categories            |String 集合                   | 包含用户与位置相关联的类别（例如，数字转换、人员）。 |
|介绍                |[positionDetail](positiondetail.md) | 包含有关用户的当前和前一个雇用职位的详细信息。                                 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workPosition",
  "baseType": ""
}-->

```json
{
  "categories": ["String"],
  "detail": {"@odata.type": "microsoft.graph.positionDetail"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workPosition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
