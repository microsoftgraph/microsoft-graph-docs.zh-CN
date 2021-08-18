---
title: accessReviewReviewer 资源类型
description: 代表为访问评审而联系的审阅者。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f5fbeda2ca839fe07009a46ab2bccd1deb502f17
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259222"
---
# <a name="accessreviewreviewer-resource-type"></a>accessReviewReviewer 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

代表为完成审阅而联系的审阅者的身份的对象。

继承自 [实体](entity.md)。

## <a name="properties"></a>属性
| 属性 | 类型 | 说明 |
| :-------------------------| :---------- | :---------- |
| createdDateTime | DateTimeOffset | 为访问评审添加审阅者的日期。 |
| displayName | String | 审阅者的名称。 |
| id | 字符串 | 审阅者的标识符。 继承自 [实体](entity.md)。 |
| userPrincipalName | 字符串 | 用户的用户主体名称。 |


## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewReviewer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewReviewer",
  "id": "String",
  "displayName": "String",
  "userPrincipalName": "String",
  "createdDateTime": "String (timestamp)",
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewReviewer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
