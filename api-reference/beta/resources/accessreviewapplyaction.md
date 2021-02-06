---
title: accessReviewApplyAction 资源类型
description: 表示访问评审实例完成后对已审阅用户要执行的操作。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7360c2a3a058eb4f884cb786c05a83efe09a6193
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133537"
---
# <a name="accessreviewapplyaction-resource-type"></a>accessReviewApplyAction 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在 [accessReviewScheduleDefinition 的 accessReviewScheduleSettings](accessreviewschedulesettings.md) 中应用操作 [的基本类](accessreviewscheduledefinition.md)。 支持的派生类型：

- **removeAccessApplyAction** 是 accessReviewApplyAction 的派生类型，指示在完成审阅后删除正在审阅的实体的访问权限。 这是 accessReviewScheduleSettings 中的 applyActions 属性的默认类型，不需要指定。

- **disableAndDeleteUserApplyAction** 是 accessReviewApplyAction 的派生类型，指示在完成审阅后禁用和删除正在审阅的用户。 这是非默认类型，需要在 accessReviewScheduleSettings 中指定。

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
