---
title: provisioningErrorInfo 资源类型
description: 描述设置事件的状态和相关错误。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: de8804ab2ae1e1e8f9516e25c0f0a5522d86a0ff2c3722fb9c10e47bc575869c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54205196"
---
# <a name="provisioningerrorinfo-resource-type"></a>provisioningErrorInfo 资源类型

命名空间：microsoft.graph


描述设置事件的状态和相关错误。 

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|additionalDetails|String|出现错误时的其他详细信息。|
|errorCategory|provisioningStatusErrorCategory|对错误代码进行分类。 可能的值是 `failure` `nonServiceFailure` `success` 、、、、 `unknownFutureValue`|
|errorCode|String|发生任何错误时的唯一错误代码。 [了解详细信息](/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
|reason|String|总结状态并说明状态发生的原因。|
|recommendedAction|String|提供相应错误的解决方法。|

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


