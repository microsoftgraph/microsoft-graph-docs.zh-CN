---
title: programControl 资源类型
description: 在 Azure AD access 评论功能中, program control 对象表示一个控件, 将访问权限链接到某个程序。
localization_priority: Normal
ms.openlocfilehash: 3d9829b8e2585d4deda95551021e2fd9b8d14c7a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563333"
---
# <a name="programcontrol-resource-type"></a>programControl 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 Azure AD [access 评论](accessreviews-root.md)功能中, program control 对象表示一个控件, 将访问权限链接到某个程序。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[创建 programControl](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   将 programControl 添加到程序中。|
|[删除 programControl](../api/programcontrol-delete.md) |     无。   |   从程序中删除 programControl。|
|[列出 programControls](../api/programcontrol-list.md) | [programControl](programcontrol.md)集合| 列出租户中所有程序之间的控件。|

## <a name="permissions"></a>权限

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | ProgramControl、ProgramControl 和所有 |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序                            | 不支持。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| `id`                     |`String`                | 程序和控件之间的链接的功能分配的标识符                                      |
| `programId`              |`String`                | 此控件所属程序的 programId。 创建时为必需项。                            |
| `controlId`              |`String`                | 控件的 controlId, 特别是 access 评审的标识符。 创建时为必需项。                                                |
| `controlTypeId`          |`String`                | programControlType 标识程序控制的类型-例如, 链接到来宾访问审阅的控件。 创建时为必需项。 |
| `displayName`            |`String`                | 控件的名称。                                                             |
| `status`                 |`String`                | 控件的生命周期状态。                                                 |
| `createdDateTime`        |`DateTimeOffset`        | 程序控件的创建日期和时间。                                        |
| `owner`                  |[userIdentity](useridentity.md)   | 创建程序控件的用户。                                               |
| `resource`               |`programResource`       | 由该程序控件的访问审核作为目标的资源、组或应用程序。                   |

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
| `program`                |[主程序](program.md)               | 此控件所属的程序。                                                |

## <a name="see-also"></a>另请参阅

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出程序的 programControls](../api/program-listcontrols.md) |      [programControl](programcontrol.md)集合| 获取程序的控件的集合。|
|[列出 programControlTypes](../api/programcontroltype-list.md) | [programControlType](programcontroltype.md)集合| 列出程序控制类型。 |

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

## <a name="the-programresource-complex-type"></a>programResource 复杂类型

程序控制对象中包含的程序资源是对作为访问评审目标的对象的引用的表示形式。

此类型将从`microsoft.graph.identity`继承并包含一个附加属性:

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| `type`               |`String`  | 资源的类型, 指示它是一个组还是一个应用程序。 |     


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
