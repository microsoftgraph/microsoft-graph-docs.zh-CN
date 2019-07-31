---
title: educationIdentityMatchingConfiguration 资源类型
description: 定义用于匹配学校数据配置文件标识的设置。 这些标识包括学生和教师。 根据这些设置, 将在目录中更新用户。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6805fabd857e4e906fa095c372632edbcc27fa28
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006386"
---
## <a name="educationidentitymatchingconfiguration-resource-type"></a>educationIdentityMatchingConfiguration 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义用于匹配学校数据配置文件标识的设置。 这些标识包括学生和教师。 根据这些设置, 将在目录中更新用户。

> **注意:** 在选择此资源时不会创建任何用户。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
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
