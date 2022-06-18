---
title: bookingCustomQuestion 资源类型
description: 表示 bookingBusiness 的自定义问题。
author: razortbone
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: cf672b93e30b6351d3f543b5cc9341d53fea1d5d
ms.sourcegitcommit: 8253b79a9fdfea723899860492219eaeb9f74e3d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2022
ms.locfileid: "66160634"
---
# <a name="bookingcustomquestion-resource-type"></a>bookingCustomQuestion 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [bookingBusiness](bookingbusiness.md) 的自定义问题。

继承自 [bookingNamedEntity](../resources/bookingnamedentity.md)。

## <a name="methods"></a>方法

| 方法                                                                         | 返回类型                                                               | Description                                                                                                       |
| :----------------------------------------------------------------------------- | :------------------------------------------------------------------------ | :---------------------------------------------------------------------------------------------------------------- |
| [列出 bookingCustomQuestions](../api/bookingbusiness-list-customquestions.md)            | [bookingCustomQuestion](../resources/bookingcustomquestion.md) 集合 | 获取 [bookingCustomQuestion](../resources/bookingcustomquestion.md) 对象及其属性的列表。    |
| [创建 bookingCustomQuestion](../api/bookingbusiness-post-customquestions.md) | [bookingCustomQuestion](../resources/bookingcustomquestion.md)            | 创建新的 [bookingCustomQuestion](../resources/bookingcustomquestion.md) 对象。                               |
| [获取 bookingCustomQuestion](../api/bookingcustomquestion-get.md)               | [bookingCustomQuestion](../resources/bookingcustomquestion.md)            | 读取 [bookingCustomQuestion 对象的](../resources/bookingcustomquestion.md) 属性和关系。 |
| [更新 bookingCustomQuestion](../api/bookingcustomquestion-update.md)         | 无     | 更新 [bookingCustomQuestion 对象的](../resources/bookingcustomquestion.md) 属性。                 |
| [删除 bookingCustomQuestion](../api/bookingcustomquestion-delete.md)         | 无                                                                      | 删除 [bookingCustomQuestion](../resources/bookingcustomquestion.md) 对象。                                  |

## <a name="properties"></a>属性

| 属性        | 类型              | Description                                                                                               |
| :-------------- | :---------------- | :-------------------------------------------------------------------------------------------------------- |
| answerInputType | answerInputType   | 预期的答案类型。 可能的值包括 `text`、`radioButton`、`unknownFutureValue`。     |
| answerOptions   | 字符串集合 | 可能的答案值列表。                                                                    |
| displayName     | String            | 问题。 继承自 [bookingNamedEntity](../resources/bookingnamedentity.md)。 |
| id              | String            | 自定义问题的 ID。 继承自 [entity](../resources/entity.md)。                           |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.bookingCustomQuestion",
  "baseType": "microsoft.graph.bookingNamedEntity",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.bookingCustomQuestion",
  "id": "String (identifier)",
  "displayName": "String",
  "answerInputType": {"@odata.type": "microsoft.graph.answerInputType"},
  "answerOptions": ["String"]
}
```
