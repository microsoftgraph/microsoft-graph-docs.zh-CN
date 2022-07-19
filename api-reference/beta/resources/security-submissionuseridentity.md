---
title: submissionUserIdentity 资源类型
description: 表示发送威胁提交的用户的标识。
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: c6f0fbd5c5f413200f358044a0bd202c0e4c031a
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856635"
---
# <a name="submissionuseridentity-resource-type"></a>submissionUserIdentity 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示发送威胁提交的用户的标识。

继承自 [标识](../resources/identity.md)。

## <a name="properties"></a>属性
| 属性    | 类型   | 说明                                                                                                    |
|:------------|:-------|:---------------------------------------------------------------------------------------------------------------|
| displayName | String | 继承自 **标识**。                                                                 |
| email       | String | 在登录 (委派令牌案例时提交提交内容的用户的电子邮件) 。 | 
| id          | String | 继承自 **标识**。  |


## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.submissionUserIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.submissionUserIdentity",
  "displayName": "String",
  "id": "String (identifier)",
  "email": "String"
}
```

