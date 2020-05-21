---
title: educationIdentityMatchingConfiguration 资源类型
description: 定义用于匹配学校数据配置文件标识的设置。 这些标识包括学生和教师。 根据这些设置，将在目录中更新用户。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: fd42bc30a1cc1cee34685bc0f33815f3a00d0120
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336019"
---
# <a name="educationidentitymatchingconfiguration-resource-type"></a>educationIdentityMatchingConfiguration 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义用于匹配学校数据配置文件标识的设置。 这些标识包括学生和教师。 根据这些设置，将在目录中更新用户。

> **注意：** 在选择此资源时不会创建任何用户。

## <a name="properties"></a>属性

| 属性 | 类型 | Description |
|:-|:-|:-|
| **matchingOptions** | [educationIdentityMatchingOptions](educationidentitymatchingoptions.md)集合 | 用户帐户与用于唯一标识要更新的用户的选项之间的映射。 |

## <a name="json-representation"></a>JSON 表示形式
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityMatchingConfiguration"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationIdentityMatchingConfiguration",
    "matchingOptions": [
        {
            "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
            "sourcePropertyName": "String",
            "targetPropertyName": "String",
            "targetDomain": "String"
        }
    ]
}
```
