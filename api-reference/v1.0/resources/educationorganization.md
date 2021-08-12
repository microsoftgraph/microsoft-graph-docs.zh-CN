---
title: educationOrganization 资源类型
description: 抽象实体，用于对教育部门内不同组织类型之间的通用性进行建模。
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: fa6d324602ba13ebe186bc0631de991e193d945757117217aa29296ee480ef74
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54130350"
---
# <a name="educationorganization-resource-type"></a>educationOrganization 资源类型

命名空间：microsoft.graph

抽象实体，用于对教育部门内不同组织类型之间的通用性进行建模。

继承自 [实体](../resources/entity.md)。

## <a name="properties"></a>属性

| 属性             | 类型                    | 说明                                                                            |
| :------------------- | :---------------------- | :------------------------------------------------------------------------------------- |
| 说明          | String                  | 组织说明。                                                              |
| displayName          | String                  | 组织显示名称。                                                             |
| externalSource       | educationExternalSource | 创建组织的来源。 可取值为：`sis`、`manual`。 |
| externalSourceDetail | String                  | 生成此资源的外部源的名称。                     |
| id                   | String                  | 对象标识符。 继承自 [实体](../resources/entity.md)                     |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationOrganization",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationOrganization",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "externalSource": "String",
  "externalSourceDetail": "String"
}
```
