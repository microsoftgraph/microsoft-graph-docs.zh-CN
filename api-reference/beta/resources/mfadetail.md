---
title: mfaDetail 资源类型
description: '指示特定登录的 MFA 详细信息。 它包括用于登录的身份验证方法以及身份验证详细信息 (例如：电话、短信或语音邮件)  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: besiler
ms.openlocfilehash: b3cd2392b9591cfb5465f2f269db547cd37754ea
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50759795"
---
# <a name="mfadetail-resource-type"></a>mfaDetail 资源类型

命名空间：microsoft.graph 指示特定登录的 MFA 详细信息。 它包括用于登录的身份验证方法以及身份验证详细信息 (例如：电话、短信或语音邮件) 



## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|authDetail|String|指示相应登录活动的 MFA 身份验证详细信息，当"需要 MFA"为"是"时。|
|authMethod|String|指示当"MFA 必填"字段 ("是"时，短信、手机、Authenticator 应用的 MFA 身份验证方法是相应登录活动的一些值) 。|

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


