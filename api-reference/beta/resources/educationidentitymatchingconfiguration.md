---
title: educationIdentityMatchingConfiguration 资源类型
description: 定义用于匹配学校数据配置文件标识的设置。 这些标识包括学生和教师。 根据这些设置，将在目录中更新用户。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 7c26ef1447272b88c59ec6992e41ae051439645e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095388"
---
# <a name="educationidentitymatchingconfiguration-resource-type"></a>educationIdentityMatchingConfiguration 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义用于匹配学校数据配置文件标识的设置。 这些标识包括学生和教师。 根据这些设置，将在目录中更新用户。

> [!NOTE]
> 在选择此资源时不会创建任何用户。

## <a name="properties"></a>属性

| 属性        | 类型                                                                                               | 说明                                                                                      |
| :-------------- | :------------------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------- |
| matchingOptions | [educationIdentityMatchingOptions](educationidentitymatchingoptions.md) 集合 | 用户帐户与用于唯一标识要更新的用户的选项之间的映射。 |

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
      "appliesTo": { "@odata.type": "microsoft.graph.educationUserRole" },
      "sourcePropertyName": "String",
      "targetPropertyName": "String",
      "targetDomain": "String"
    }
  ]
}
```


