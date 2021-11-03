---
title: validationResult 资源类型
description: 公开用于指定验证用户密码的规则的属性，以及验证结果。
author: yyuank
ms.localizationpriority: medium
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 2e77770749ba06fed83e2855ff465922420da988
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60689238"
---
# <a name="validationresult-resource-type"></a>validationResult 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

公开用于指定验证用户密码的规则的属性，以及验证结果。

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|message|String| 包含规则通过原因的字符串。 只读。 不可为 null。|
|ruleName|String| 包含验证操作时所针对的密码验证规则的名称的字符串。 只读。 不可为 null。|
|validationPassed|布尔值| 密码通过还是未通过验证规则。 只读。 不可为 null。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.validationResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.validationResult",
  "ruleName": "String",
  "validationPassed": "Boolean",
  "message": "String"
}
```

