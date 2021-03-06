---
title: signInStatus 资源类型
description: 提供登录状态 (登录成功) 失败状态
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: SarahBar
ms.openlocfilehash: d7428c2a73d0b4a114599dad8ac1740d91ba5865
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132634"
---
# <a name="signinstatus-resource-type"></a>signInStatus 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供登录状态 (登录成功) 失败状态



## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|additionalDetails|字符串|提供有关登录活动的其他详细信息|
|errorCode|Int32|提供登录失败期间生成的 5-6 位数字错误代码。 查看 [错误代码和消息的列表](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)。|
|failureReason|String|提供相应登录活动的错误消息或失败原因。 查看 [错误代码和消息的列表](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInStatus"
}-->

```json
{
  "additionalDetails": "String",
  "errorCode": 1024,
  "failureReason": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


