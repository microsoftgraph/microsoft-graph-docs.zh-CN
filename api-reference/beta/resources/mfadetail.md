---
title: mfaDetail 资源类型
description: '指示特定登录的 MFA 详细信息。 它包括用于登录的身份验证方法以及身份验证详细信息 (例如：电话、短信或语音邮件)  '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: besiler
ms.openlocfilehash: 52ad666182e1ab404ba611e4ca2668745a8539fc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59100706"
---
# <a name="mfadetail-resource-type"></a>mfaDetail 资源类型

命名空间：microsoft.graph 指示特定登录的 MFA 详细信息。 它包括用于登录的身份验证方法以及身份验证详细信息 (例如：电话、短信或语音邮件) 



## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|authDetail|String|指示相应登录活动的 MFA 身份验证详细信息，当"需要 MFA"为"是"时。|
|authMethod|String|指示当"MFA 必填"字段为"是"时， (短信、电话、Authenticator 应用的 MFA 身份验证方法是相应登录活动的一些值) 。|

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


