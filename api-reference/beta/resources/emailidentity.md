---
title: emailIdentity 资源类型
description: 表示用户的电子邮件标识。
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 90882a78c149e089fd00baa266240cb574e9864a
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979547"
---
# <a name="emailidentity-resource-type"></a>emailIdentity 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用户的电子邮件标识。


继承自 [标识](../resources/identity.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|字符串|用户的显示名称。 继承自 [标识](../resources/identity.md)。|
|email|字符串|用户的电子邮件地址。|
|id|字符串|用户的 ID。 继承自 [标识](../resources/identity.md)。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.emailIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "email": "String"
}
```

