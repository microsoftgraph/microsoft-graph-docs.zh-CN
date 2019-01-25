---
title: 计划资源类型
description: '在 Azure AD 中访问审阅功能，程序是容器，保存程序控件。 租户可以有一个或多个程序。  每个控件链接到程序访问检查，以使其更轻松地找到相关的 access 审阅。  '
localization_priority: Normal
ms.openlocfilehash: 2498279f27f5859eadcfa1d70662e3d8f3b5246c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515186"
---
# <a name="program-resource-type"></a>计划资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 Azure AD[访问审阅](accessreviews-root.md)功能中，程序是容器，保存程序控件。 租户可以有一个或多个程序。  每个控件链接到程序访问检查，以使其更轻松地找到相关的 access 审阅。  

已在-boarded Azure AD 每个租户访问评论具有一个程序`Default program`。  全局管理员可以创建其他程序，例如表示法规遵从性计划。 


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[创建程序](../api/program-create.md) |   [程序](program.md)   |   创建一个新的程序。|
|[删除程序](../api/program-delete.md) |   无。   |   删除一个程序。|
|[列表程序](../api/program-list.md) |  [程序](program.md)集|   获取所有的程序的集合。|
|[对程序的列表 programControls](../api/program-listcontrols.md) |      [programControl](programcontrol.md)集合| 获取一个程序的控件的集合。|
|[更新程序](../api/program-update.md) |   [程序](program.md)|  更新程序。|

## <a name="permissions"></a>权限

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | ProgramControl.Read.All ProgramControl.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序                            | 不支持。 |


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  功能分配的程序标识符。                    |
| `displayName`               |`String`                              |  程序的名称。  所需在创建。                  |
| `description`               |`String`                              |  该程序的描述。           |

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
| `controls`                  |[programControl](programcontrol.md) | 程序相关联的控件。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/program.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
