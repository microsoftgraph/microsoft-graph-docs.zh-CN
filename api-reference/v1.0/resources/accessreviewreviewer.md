---
title: accessReviewReviewer 资源类型
description: 代表为访问评审而联系的审阅者。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3a2a51908f73278e592ec02852c96f75570b7646
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/21/2022
ms.locfileid: "62162120"
---
# <a name="accessreviewreviewer-resource-type"></a>accessReviewReviewer 资源类型

命名空间：microsoft.graph

表示为完成审阅而联系的审阅者的身份。

继承自 [实体](entity.md)。

## <a name="properties"></a>属性
| 属性 | 类型 | 说明 |
| :-------------------------| :---------- | :---------- |
| createdDateTime | DateTimeOffset | 为访问评审添加审阅者的日期。 |
| displayName | String | 审阅者的名称。 |
| id | String | 审阅者的标识符。 继承自 [实体](entity.md)。 |
| userPrincipalName | String | 审阅者的用户主体名称。 |


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
