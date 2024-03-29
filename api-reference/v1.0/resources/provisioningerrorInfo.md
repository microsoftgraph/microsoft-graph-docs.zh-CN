---
title: provisioningErrorInfo 资源类型
description: 描述设置事件的状态和相关错误。
ms.localizationpriority: medium
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: f0b6e42fc184db1d8c2044d56820d0e19e89f8c3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019165"
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


