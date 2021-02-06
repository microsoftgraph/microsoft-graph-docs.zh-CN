---
title: accessPackageAnswer 资源类型
description: 存储在 accessPackageAssignmentRequest 上的 accessPackageQuestion 答案的复杂类型。
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3da6d1b0e2e519895af4dacca009b027807b0184
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135494"
---
# <a name="accesspackageanswer-resource-type"></a>accessPackageAnswer 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

请求者提供的 [accessPackageQuestion](../resources/accesspackagequestion.md)答案的复杂类型。 实际答案将是此复杂类型的子类型，[即 accessPackageAnswerString](../resources/accesspackageanswerstring.md)或[accessPackageAnswerChoice。](../resources/accesspackageanswerchoice.md) 这些答案将存储在 [accessPackageAssignmentRequest 上](../resources/accesspackageassignmentrequest.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|answeredQuestion|[accessPackageQuestion](../resources/accesspackagequestion.md)|答案针对的问题。 必需且只读。|
|displayValue|字符串|答案的显示值。 必填。|

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

