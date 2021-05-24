---
title: provisioningErrorInfo 资源类型
description: 描述设置事件的状态和相关错误。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: a682e176b40d58e2dc0a794b58b8561f8948d5a5
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547153"
---
# <a name="provisioningerrorinfo-resource-type"></a>provisioningErrorInfo 资源类型

命名空间：microsoft.graph


描述设置事件的状态和相关错误。 

## <a name="properties"></a>属性

| 属性     | 类型        | 描述 |
|:-------------|:------------|:------------|
|additionalDetails|字符串|出现错误时的其他详细信息。|
|errorCategory|provisioningStatusErrorCategory|对错误代码进行分类。 可能的值是 `failure` `nonServiceFailure` `success` 、、、、 `unknownFutureValue`|
|errorCode|String|发生任何错误时的唯一错误代码。 [了解更多](/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
|reason|字符串|总结状态并说明状态发生的原因。|
|recommendedAction|字符串|提供相应错误的解决方法。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningErrorInfo",
  "baseType": null
}-->

```json
{
  "additionalDetails": "String",
  "errorCategory": "String",
  "errorCode": "String",
  "reason": "String",
  "recommendedAction": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningErrorInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


