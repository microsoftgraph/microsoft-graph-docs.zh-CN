---
title: programControl 资源类型
description: 在 Azure AD 中访问审阅功能，程序 control 对象代表链接到程序访问审阅的一个控件。
localization_priority: Normal
ms.openlocfilehash: 82d9263a909fb11e688ffa6b27f0cf92601ae9e9
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576554"
---
# <a name="programcontrol-resource-type"></a>programControl 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 Azure AD[访问审阅](accessreviews-root.md)功能中，程序控件对象表示的控件，将访问审阅链接到一个程序。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[创建 programControl](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   添加到程序 programControl。|
|[删除 programControl](../api/programcontrol-delete.md) |     无。   |   从某个程序中删除 programControl。|
|[列表 programControls](../api/programcontrol-list.md) | [programControl](programcontrol.md)集合| 在租户中的所有程序列表控件中。|

## <a name="permissions"></a>权限

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | ProgramControl.Read.All ProgramControl.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序                            | 不支持。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| `id`                     |`String`                | 功能指派的标识符的程序和控件之间的链接                                      |
| `programId`              |`String`                | 程序 programId 此控件是组成部分。 所需在创建。                            |
| `controlId`              |`String`                | 控件的 controlId，尤其要指出的访问的标识符查看。 所需在创建。                                                |
| `controlTypeId`          |`String`                | ProgramControlType 标识的程序控件的类型-例如，将链接到来宾访问控制审阅。 所需在创建。 |
| `displayName`            |`String`                | 控件的名称。                                                             |
| `status`                 |`String`                | 控件的生命周期状态。                                                 |
| `createdDateTime`        |`DateTimeOffset`        | 创建日期和时间的程序控制。                                        |
| `owner`                  |[userIdentity](useridentity.md)   | 创建程序控制的用户。                                               |
| `resource`               | [programResource](programresource.md)       | 资源、 组或应用程序，此程序控制访问审阅的目标。                   |

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
| `program`                |[程序](program.md)               | 此控件属于该程序。                                                |

## <a name="see-also"></a>另请参阅

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[对程序的列表 programControls](../api/program-listcontrols.md) |      [programControl](programcontrol.md)集合| 获取一个程序的控件的集合。|
|[列表 programControlTypes](../api/programcontroltype-list.md) | [programControlType](programcontroltype.md)集合| 列出程序控件类型。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programControl"
}-->

```json
{
 "id": "string (identifier)",
 "programId": "string (identifier)",
 "controlId": "string (identifier)",
 "controlTypeId": "string (identifier)",
 "displayName": "string",
 "status": "string",
 "createdDateTime": "string (timestamp)",
 "owner": "microsoft.graph.userIdentity",
 "resource":"microsoft.graph.programResource"
}

```

## <a name="the-programresource-complex-type"></a>ProgramResource 复杂类型

包含程序 control 对象，该程序资源是引用的对目标的访问审阅的对象的表示形式。

此类型继承自`microsoft.graph.identity`，并且具有一个附加属性：

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| `type`               |`String`  | 资源，指明它一组或应用程序的类型。 |     


<!--
{
  "type": "#page.annotation",
  "description": "programControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/programcontrol.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
