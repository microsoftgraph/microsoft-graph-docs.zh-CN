---
title: accessReviewApplyAction 资源类型
description: 表示在访问评审实例完成后要对已审阅用户执行的操作。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: aed70bb75bd690ec8532727b90954b23e927f16e
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697251"
---
# <a name="accessreviewapplyaction-resource-type"></a>accessReviewApplyAction 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

表示在 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 对象的 [accessReviewScheduleSettings](accessreviewschedulesettings.md) 中应用操作的基类。 支持以下派生类型：

- [removeAccessApplyAction](removeaccessapplyaction.md) 指示在审阅完成后删除正在审查的实体的访问权限。 这是 accessReviewScheduleSettings 中 applyActions 属性的默认类型，无需指定。

- [disableAndDeleteUserApplyAction](disableanddeleteuserapplyaction.md) 指示在审阅完成后禁用和删除正在审阅的用户。 这是非默认类型，必须在 accessReviewScheduleSettings 中显式指定。

## <a name="properties"></a>属性
无。

## <a name="relationships"></a>关系
无。


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewApplyAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewApplyAction"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewApplyAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
