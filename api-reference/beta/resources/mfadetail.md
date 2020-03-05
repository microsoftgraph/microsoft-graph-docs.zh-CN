---
title: mfaDetail 资源类型
description: '指示特定登录的 MFA 详细信息。 它包括用于登录的身份验证方法以及身份验证的详细信息（例如：电话、短信或语音邮件） '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 15c15d3ec6db5acb16387a4b76501229167b0912
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522643"
---
# <a name="mfadetail-resource-type"></a>mfaDetail 资源类型

命名空间： microsoft. graph 指示特定登录的 MFA 详细信息。 它包括用于登录的身份验证方法以及身份验证的详细信息（例如：电话、短信或语音邮件） 



## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|authDetail|String|当所需的 MFA 为 "是" 时，指示对应登录活动的 MFA 身份验证详细信息。|
|authMethod|String|指示当 "MFA 必需" 字段为 "是" 时，对相应登录活动的 MFA 身份验证方法（SMS、电话、验证器应用程序值）。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mfaDetail"
}-->

```json
{
  "authDetail": "String",
  "authMethod": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mfaDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
