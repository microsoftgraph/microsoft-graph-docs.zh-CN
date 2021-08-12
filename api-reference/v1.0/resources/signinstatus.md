---
title: signInStatus 资源类型
description: 提供登录状态 (登录的成功) 失败状态
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 350ed66245164b5745d7b6f0bc962ebab5b1b4e46e8d7fc6b9a5c45b17ccc3a1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54222670"
---
# <a name="signinstatus-resource-type"></a>signInStatus 资源类型

命名空间：microsoft.graph

提供登录的登录 (登录) 失败或失败状态。

## <a name="properties"></a>属性

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|additionalDetails|String|提供有关登录活动的其他详细信息|
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

