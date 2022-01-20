---
title: governanceInsight 资源类型
description: 表示向 accessReviewInstanceDecisionItem 的审阅者呈现的见解。
author: shubhamguptacal
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: fdbe8aa65487e1d872e7f0943ae5582958fcaaec
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137249"
---
# <a name="governanceinsight-resource-type"></a>governanceInsight 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

表示向 [accessReviewInstanceDecisionItem 的审阅者呈现的见解](accessreviewinstancedecisionitem.md)。 Insights审阅者的建议，以帮助他们完成访问评审。

此资源是 [userSignInInsight 派生](usersignininsight.md) 类型的抽象类型。

## <a name="properties"></a>属性
| 属性    | 类型   | 说明 |
| :---------------| :---------- | :---------- |
| id | String | 见解的标识符。 只读。 |
| insightCreatedDateTime | DateTimeOffset | 指示创建见解时。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.governanceInsight",
  "keyProperty": "id"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.governanceinsight",
  "id": "String",
  "insightCreatedDateTime": "DateTimeOffset"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "governanceinsight resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
