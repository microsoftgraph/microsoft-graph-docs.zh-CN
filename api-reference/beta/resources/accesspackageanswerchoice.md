---
title: accessPackageAnswerChoice 资源类型
description: accessPackageMultipleChoiceQuestion 的应答选项。
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6f34656a72d217adec1ff46be689b283461332fb
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720147"
---
# <a name="accesspackageanswerchoice-resource-type"></a>accessPackageAnswerChoice 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指示 [accessPackageMultipleChoiceQuestion](../resources/accesspackagemultiplechoicequestion.md)的应答选项。 可以将多个 accessPackageAnswerChoices 添加到 [accessPackageMultipleChoiceQuestion](../resources/accesspackagemultiplechoicequestion.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|actualValue|String|所选实际值的项。 这通常是应用程序可以理解的字符串值。 必需。 |
|displayValue|[accessPackageLocalizedContent](../resources/accesspackagelocalizedcontent.md)|向请求者和审批者显示的本地化显示值。 必填。

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAnswerChoice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAnswerChoice",
  "actualValue": "String",
  "displayValue": {
    "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
  }
}
```
