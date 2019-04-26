---
title: 程序资源类型
description: '在 Azure AD access 评论功能中, 程序是容器, 保留程序控件。 一个租户可以有一个或多个程序。  每个控件都将访问审核链接到某个程序, 以便更轻松地找到相关的访问评审。  '
localization_priority: Normal
ms.openlocfilehash: 7c0016cb194acd7ad8533acb34650b57df720ace
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344017"
---
# <a name="program-resource-type"></a>程序资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 Azure AD [access 评论](accessreviews-root.md)功能中, 程序是容器, 保留程序控件。 一个租户可以有一个或多个程序。  每个控件都将访问审核链接到某个程序, 以便更轻松地找到相关的访问评审。  

每个具有 boarded Azure AD access 评审的租户都有一个程序`Default program`。  全局管理员可以创建其他程序, 例如表示合规性计划。 


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[创建程序](../api/program-create.md) |   [主程序](program.md)   |   创建新程序。|
|[删除程序](../api/program-delete.md) |   无。   |   删除程序。|
|[列出程序](../api/program-list.md) |  [程序](program.md)集|   获取所有程序的集合。|
|[列出程序的 programControls](../api/program-listcontrols.md) |      [programControl](programcontrol.md)集合| 获取程序的控件的集合。|
|[更新程序](../api/program-update.md) |   [主程序](program.md)|  更新程序。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  功能分配的程序标识符。                    |
| `displayName`               |`String`                              |  程序的名称。  创建时为必需项。                  |
| `description`               |`String`                              |  程序的说明。           |

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
| `controls`                  |[programControl](programcontrol.md) | 与该程序关联的控件。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.program"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string",
 "description": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "program resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
