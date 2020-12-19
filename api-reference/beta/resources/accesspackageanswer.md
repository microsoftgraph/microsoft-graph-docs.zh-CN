---
title: accessPackageAnswer 资源类型
description: 存储在 accessPackageAssignmentRequest 上的 accessPackageQuestion 答案的复杂类型。
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f947c5235c18d3be5115199d789512602a3e0739
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720135"
---
# <a name="accesspackageanswer-resource-type"></a>accessPackageAnswer 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

请求者提供的 [accessPackageQuestion](../resources/accesspackagequestion.md)答案的复杂类型。 实际答案将是此复杂类型的子类型，[即 accessPackageAnswerString](../resources/accesspackageanswerstring.md)或[accessPackageAnswerChoice。](../resources/accesspackageanswerchoice.md) 这些答案将存储在 [accessPackageAssignmentRequest 上](../resources/accesspackageassignmentrequest.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|answeredQuestion|[accessPackageQuestion](../resources/accesspackagequestion.md)|答案针对的问题。 必需且只读。|
|displayValue|String|答案的显示值。 必填。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAnswer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAnswer",
  "displayValue": "String",
  "answeredQuestion": {
    "@odata.type": "microsoft.graph.accessPackageQuestion"
  }
}
```

