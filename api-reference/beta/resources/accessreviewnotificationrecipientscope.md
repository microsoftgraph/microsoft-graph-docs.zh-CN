---
title: accessreviewnotificationrecipientscope 资源类型
description: 表示将接收访问评审通知的人员。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 82aa0a4ebb164028c33bf05b4802774a81a18907
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698115"
---
# <a name="accessreviewnotificationrecipientscope-resource-type"></a>accessreviewnotificationrecipientscope 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

**accessReviewNotificationRecipientScope** 表示一个基类，用于定义将接收 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 对象实例通知的用户。 它由 [accessReviewNotificationRecipientQueryScope](../resources/accessReviewNotificationRecipientQueryScope.md) 继承。
## <a name="properties"></a>属性
无。

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewNotificationRecipientScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewNotificationRecipientScope"
}
```