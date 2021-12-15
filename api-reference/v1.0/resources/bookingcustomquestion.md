---
title: bookingCustomQuestion 资源类型
description: 表示 bookingBusiness 的自定义问题。
author: razortbone
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 9a9f88d7ee5fe20d1dc5b4033353b2ac7b744878
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525025"
---
# <a name="bookingcustomquestion-resource-type"></a>bookingCustomQuestion 资源类型

命名空间：microsoft.graph

表示 [bookingBusiness 的自定义问题](bookingbusiness.md)。

## <a name="methods"></a>方法

| 方法                                                                         | 返回类型                                                               | 说明                                                                                                       |
| :----------------------------------------------------------------------------- | :------------------------------------------------------------------------ | :---------------------------------------------------------------------------------------------------------------- |
| [列出 bookingCustomQuestions](../api/bookingbusiness-list-customquestions.md)  | [bookingCustomQuestion](../resources/bookingcustomquestion.md) 集合 | 获取 [bookingCustomQuestion](../resources/bookingcustomquestion.md) 对象及其属性的列表。    |
| [创建 bookingCustomQuestion](../api/bookingbusiness-post-customquestions.md) | [bookingCustomQuestion](../resources/bookingcustomquestion.md)            | 创建新的 [bookingCustomQuestion](../resources/bookingcustomquestion.md) 对象。                               |
| [获取 bookingCustomQuestion](../api/bookingcustomquestion-get.md)               | [bookingCustomQuestion](../resources/bookingcustomquestion.md)            | 读取 [bookingCustomQuestion](../resources/bookingcustomquestion.md) 对象的属性和关系。 |
| [更新 bookingCustomQuestion](../api/bookingcustomquestion-update.md)         | [bookingCustomQuestion](../resources/bookingcustomquestion.md)            | 更新 [bookingCustomQuestion 对象](../resources/bookingcustomquestion.md) 的属性。                 |
| [删除 bookingCustomQuestion](../api/bookingcustomquestion-delete.md)         | 无                                                                      | 删除 [bookingCustomQuestion](../resources/bookingcustomquestion.md) 对象。                                  |

## <a name="properties"></a>属性

| 属性        | 类型              | 说明                                                                                               |
| :-------------- | :---------------- | :-------------------------------------------------------------------------------------------------------- |
| answerInputType | answerInputType   | 预期的答案类型。 可能的值包括 `text`、`radioButton`、`unknownFutureValue`。     |
| answerOptions   | String collection | 可能的答案值列表。                                                                    |
| displayName     | String            | 问题。 |
| id              | String            | 自定义问题的 ID。 继承自 [实体](../resources/entity.md)。                           |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.bookingCustomQuestion",
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
