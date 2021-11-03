---
title: passwordValidationInformation 资源类型
description: 公开指定在针对租户的密码验证策略验证用户密码时用户密码是否有效的属性。
author: yyuank
ms.localizationpriority: medium
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 0da72df7551b84284dc9caa7d9183ef31834eba7
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60689241"
---
# <a name="passwordvalidationinformation-resource-type"></a>passwordValidationInformation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

公开一些属性，这些属性指定在针对租户的密码验证策略验证用户密码时用户密码是否有效。 此资源还返回验证密码的规则列表，以及用户的密码是否传递了这些角色。


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|isValid|布尔值| 根据 **validationResults** 属性中的结果计算指定密码是否有效。 不可为 null。 只读。 |
|validationResults|[validationResult](../resources/validationresult.md) 集合| 密码验证规则列表以及密码是否通过了这些规则。 不可为 null。 只读。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.passwordValidationInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordValidationInformation",
  "isValid": "Boolean",
  "validationResults": [
    {
      "@odata.type": "microsoft.graph.validationResult"
    }
  ]
}
```

