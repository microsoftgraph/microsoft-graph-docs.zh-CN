---
title: accessPackageAnswerChoice 资源类型
description: accessPackageMultipleChoiceQuestion 的应答选项。
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7c7fc7db1c9360146c2f62fd9048ad0db3d58b80
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135476"
---
# <a name="accesspackageanswerchoice-resource-type"></a>accessPackageAnswerChoice 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指示 [accessPackageMultipleChoiceQuestion](../resources/accesspackagemultiplechoicequestion.md)的应答选项。 可以将多个 accessPackageAnswerChoices 添加到 [accessPackageMultipleChoiceQuestion](../resources/accesspackagemultiplechoicequestion.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|actualValue|字符串|所选实际值的项。 这通常是应用程序可以理解的字符串值。 必填。 |
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
