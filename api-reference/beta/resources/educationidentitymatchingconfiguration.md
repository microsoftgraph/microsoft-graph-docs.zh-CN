---
title: educationIdentityMatchingConfiguration 资源类型
description: 用于匹配学校数据配置文件标识中定义的设置。 这些身份包括学生和教师。 根据这些设置，用户将更新目录中。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9ee9f58c2f69882361ee105a1d7531bb5756e165
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977547"
---
## <a name="educationidentitymatchingconfiguration-resource-type"></a>educationIdentityMatchingConfiguration 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

用于匹配学校数据配置文件标识中定义的设置。 这些身份包括学生和教师。 根据这些设置，用户将更新目录中。

> **注意：** 选择此资源时，会不创建任何用户。

## <a name="properties"></a>属性

| 属性 | 类型 | Description |
|:-|:-|:-|
| **matchingOptions** | [educationIdentityMatchingOptions](educationidentitymatchingoptions.md)集合 | 用户帐户和选项用于唯一标识用户更新之间的映射。 |

## <a name="json-representation"></a>JSON 表示形式
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityMatchingConfiguration"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationIdentityMatchingConfiguration",
    "matchingOptions": [
        {
            "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
            "sourcePropertyName": "String",
            "targetPropertyName": "String",
            "targetDomain": "String"
        }
    ]
}
```
