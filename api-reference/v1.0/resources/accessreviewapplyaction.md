---
title: accessReviewApplyAction 资源类型
description: 表示访问评审实例完成后对被审阅用户要执行的操作。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8c887c1b2bbef46f963e2260f4bfe99215cddc2d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59021762"
---
# <a name="accessreviewapplyaction-resource-type"></a>accessReviewApplyAction 资源类型

命名空间：microsoft.graph

表示在 [accessReviewScheduleDefinition 的 accessReviewScheduleSettings](accessreviewschedulesettings.md) 中应用操作 [的基本类](accessreviewscheduledefinition.md)。 支持的派生类型：

- [removeAccessApplyAction](removeaccessapplyaction.md) 是 accessReviewApplyAction 的派生类型，指示在完成审阅后删除正在审阅的实体的访问权限。 这是 accessReviewScheduleSettings 中 applyActions 属性的默认类型，不需要指定。

- [disableAndDeleteUserApplyAction](disableanddeleteuserapplyaction.md) 是 accessReviewApplyAction 的派生类型，指示在完成审阅后禁用和删除正在审阅的用户。 这是非默认类型，需要在 accessReviewScheduleSettings 中指定。

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

