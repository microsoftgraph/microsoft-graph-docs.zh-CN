---
title: accessReviewApplyAction 资源类型
description: 表示在完成访问审核实例后要对审阅的用户执行的操作。
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 33aa0f7a9d7fbfeab9b957f4c94b87d6f6e50d44
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000832"
---
# <a name="accessreviewapplyaction-resource-type"></a>accessReviewApplyAction 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在[accessReviewScheduleDefinition](accessreviewscheduledefinition.md)的[accessReviewScheduleSettings](accessreviewschedulesettings.md)中应用操作的基类。 支持的派生类型：

- **removeAccessApplyAction** 是 accessReviewApplyAction 的派生类型，它指示删除完成评审时审阅的实体的访问权限。 这是 accessReviewScheduleSettings 中 applyActions 属性的默认类型，无需指定。

- **disableAndDeleteUserApplyAction** 是 accessReviewApplyAction 的派生类型，它指示在完成审阅时禁用和删除要审阅的用户。 这是非默认类型，需要在 accessReviewScheduleSettings 中指定。

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
