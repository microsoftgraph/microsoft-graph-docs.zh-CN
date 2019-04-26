---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: RestoreAction
localization_priority: Normal
ms.openlocfilehash: f04f9811cefba60d0b06b99605774fb8fbfa0125
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562970"
---
# <a name="restoreaction-resource-type"></a>RestoreAction 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[**itemActivity**][activity] 上存在 **RestoreAction** 资源指示活动还原了一个项。

**注意**：尽管此资源暂为空，但在今后推出的 API 版本中将在此资源中填充其他属性。

[activity]: itemactivity.md

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.restoreAction"
}-->

```json
{
}
```

## <a name="properties"></a>属性

无。 此 Facet 的值可以为 null，也可以不为 null，但不含任何属性。

## <a name="remarks"></a>注解

项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。

<!--
{
  "type": "#page.annotation",
  "description": "The RestoreAction object provides information about an activity that restored an item.",
  "keywords": "activities,activity,action,restore,undelete",
  "section": "documentation",
  "tocPath": "Resources/RestoreAction",
  "suppressions": []
}
-->
