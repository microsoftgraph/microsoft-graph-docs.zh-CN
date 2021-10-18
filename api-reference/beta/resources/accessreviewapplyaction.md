---
title: accessReviewApplyAction 资源类型
description: 表示访问评审实例完成后对被审阅用户要执行的操作。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 549fbdf4394d04297fe5fc8045ccd63eb5741128
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60454031"
---
# <a name="accessreviewapplyaction-resource-type"></a>accessReviewApplyAction 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

表示在[accessReviewScheduleDefinition](accessreviewscheduledefinition.md)对象的[accessReviewScheduleSettings 中](accessreviewschedulesettings.md)应用操作的基本类。 支持以下派生类型：

- [removeAccessApplyAction](removeaccessapplyaction.md) 指示在完成审阅后删除正在审阅的实体的访问权限。 这是 accessReviewScheduleSettings 中 applyActions 属性的默认类型，不需要指定。

- [disableAndDeleteUserApplyAction](disableanddeleteuserapplyaction.md) 指示在完成审阅后禁用和删除正在审阅的用户。 这是非默认类型，必须在 accessReviewScheduleSettings 中显式指定。

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
