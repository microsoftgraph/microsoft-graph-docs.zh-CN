---
title: accessReviewReviewer 资源类型
description: 表示已联系其进行访问评审的审阅者。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ab365ee1d3b3fd53696e8fa92a2aa25dfdfd0a97
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698413"
---
# <a name="accessreviewreviewer-resource-type"></a>accessReviewReviewer 资源类型

命名空间：microsoft.graph

表示被联系以完成审阅的审阅者的身份。

继承自 [entity](entity.md)。

## <a name="properties"></a>属性
| 属性 | 类型 | 说明 |
| :-------------------------| :---------- | :---------- |
| createdDateTime | DateTimeOffset | 为访问评审添加审阅者时的日期。 |
| displayName | 字符串 | 审阅者的名称。 |
| id | String | 审阅者的标识符。 继承自 [entity](entity.md)。 |
| userPrincipalName | 字符串 | 审阅者的用户主体名称。 |


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
