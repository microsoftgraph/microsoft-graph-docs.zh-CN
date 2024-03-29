---
title: '程序资源类型 (已弃用) '
description: '在 Azure AD 访问评审功能中，程序是一个容器，包含程序控件。 租户可以有一个或多个程序。  每个控件将访问评审链接到某个程序，以便更轻松地查找相关的访问评审。  '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: f0d0a7a42a21a95bbf57b971d09e20046bd46ffa
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819396"
---
# <a name="program-resource-type-deprecated"></a>程序资源类型 (已弃用) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

在 Azure AD [访问评审](accessreviews-root.md) 功能中，程序是一个容器，包含程序控件。 租户可以有一个或多个程序。  每个控件将访问评审链接到某个程序，以便更轻松地查找相关的访问评审。  

每个已加入 Azure AD 访问评审的租户都有一个计划 `Default program`。  全局管理员可以创建其他程序，例如表示合规性计划。 


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[创建程序](../api/program-create.md) |   [程序](program.md)   |   创建新程序。|
|[删除程序](../api/program-delete.md) |   无。   |   删除程序。|
|[列出程序](../api/program-list.md) |  [程序](program.md) 集合|   获取所有程序的集合。|
|[列出程序的 programControls](../api/program-listcontrols.md) |      [programControl](programcontrol.md) 集合| 获取程序控件的集合。|
|[更新程序](../api/program-update.md) |   [程序](program.md)|  更新程序。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| id                        |String                              |  程序的功能分配标识符。                    |
| displayName               |String                              |  程序的名称。  创建时为必需项。                  |
| 说明               |String                              |  程序的说明。           |

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
| `controls`                  |[programControl](programcontrol.md) | 与程序关联的控件。 |

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


