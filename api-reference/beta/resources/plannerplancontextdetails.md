---
title: plannerPlanContextDetails 资源类型
description: '**plannerPlanContextDetails** 资源包含有关 plannerPlanContext 的其他信息。'
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: bdb65fab6aecf9c61e066c7e80e9226220c3491c
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63367921"
---
# <a name="plannerplancontextdetails-resource-type"></a>plannerPlanContextDetails 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**plannerPlanContextDetails** 资源包含有关 [plannerPlanContext 的其他信息](plannerplancontext.md)。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|customLinkText|String|可为 NULL。 指定在用户体验中用于显示链接的相关 [plannerPlanContext 的文本](plannerplancontext.md)。 如果为 null，应用程序应基于 **displayLinkType** 属性显示包含自定义文本的链接。|
|displayLinkType|plannerPlanContextType|指定应用程序如何显示指向关联的 **plannerPlanContext 的链接**。 应用程序可以选择根据链接类型提供自定义文本、说明、图标或其他体验。 可取值为：`teamsTab`、`sharePointPage`、`meetingNotes`、`other`、`unknownFutureValue`。|
|url|String|由关联的 **plannerPlanContext 表示的用户体验的** URL。 |
|state|plannerContextState| 指示关联的 **plannerPlanContext 的状态**。 |

### <a name="plannercontextstate-values"></a>plannerContextState 值

|值              |说明|
|:------------------|:----------------------------------------------------------------------|
|active             | 上下文没有问题。                                          |
|已取消链接           | 以前链接的 **plannerPlanContext** 不再链接到计划。 |
|unknownFutureValue | 可发展枚举 sentinel 值。 请勿使用。                     |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.plannerPlanContextDetails"
}-->

```json
{
  "url": "string",
  "customLinkText": "string",
  "displayLinkType": "string",
  "state": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


