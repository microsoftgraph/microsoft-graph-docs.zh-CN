---
title: mfaDetail 资源类型
description: '指示 MFA 特定登录的详细信息。 它包括用于登录以及身份验证的详细信息的身份验证方法 (例如： 电话、 SMS 或语音邮件) '
localization_priority: Normal
ms.openlocfilehash: 5069045fd202d443a94a80f7333f12ab5e707ada
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883739"
---
# <a name="mfadetail-resource-type"></a>mfaDetail 资源类型
指示 MFA 特定登录的详细信息。 它包括用于登录以及身份验证的详细信息的身份验证方法 (例如： 电话、 SMS 或语音邮件) 



## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|authDetail|字符串|指示相应的登录活动的 MFA 身份验证的详细的信息时所需 MFA 为"Yes"。|
|身份验证方法|字符串|所需的 MFA 字段为"Yes"时对相应的登录活动，指示 MFA 身份验证方法 （SMS、 电话、 Authenticator 应用程序是一些值的）。|

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
