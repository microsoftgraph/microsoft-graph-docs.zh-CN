---
title: programControl 资源类型
description: 在 Azure AD 访问评审功能中，程序控制对象表示一个控件，将访问评审链接到某个程序。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 492dc57bfa332472cb7565580ffaa8a5260234c0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443977"
---
# <a name="programcontrol-resource-type"></a>programControl 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 Azure AD [访问评审](accessreviews-root.md) 功能中，程序控制对象表示一个控件，将访问评审链接到某个程序。


## <a name="methods"></a>Methods

| 方法 | 返回类型 | 说明 |
|:------ |:----------- |:----------- |
| [创建 programControl](../api/programcontrol-create.md) |    [programControl](programcontrol.md) |   将 programControl 添加到程序。 |
| [删除 programControl](../api/programcontrol-delete.md) | 无。 | 从程序中删除 programControl。 |
| [列出 programControls](../api/programcontrol-list.md) | [programControl](programcontrol.md) 集合 | 列出租户中所有程序控件。 |
| [列出程序的 programControls](../api/program-listcontrols.md) | [programControl](programcontrol.md) 集合 |    获取程序控件的集合。 |
| [列出 programControlTypes](../api/programcontroltype-list.md) | [programControlType](programcontroltype.md) 集合| 列出程序控件类型。 |

## <a name="properties"></a>属性

| 属性 | 类型   | 说明 |
|:-------- |:---- |:----------- |
| id | String | 程序与控件之间的链接的功能分配标识符。 |
| programId | String | 此控件是程序的 programId 的一部分。 创建时为必需项。 |
| controlId | String | 控件的 controlId，尤其是访问评审的标识符。 创建时为必需项。 |
| controlTypeId | String | programControlType 标识程序控件的类型-例如，链接到来宾访问评审的控件。 创建时为必需项。 |
| displayName | String | 控件的名称。 |
| status | String | 控件的生命周期状态。 |
| createdDateTime | DateTimeOffset | 程序控件的创建日期和时间。 |
| 所有者 | [userIdentity](useridentity.md) | 创建程序控件的用户。 |
| resource | [programResource](programresource.md) | 此程序控件的访问评审针对的资源、组或应用。 |

## <a name="relationships"></a>关系

| 关系 | 类型   | 说明 |
|:------------ |:---- |:----------- |
| program | [program](program.md) | 此控件属于的程序。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
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
 "owner": {"@odata.type":"microsoft.graph.userIdentity"},
 "resource":{"@odata.type":"microsoft.graph.programResource"}
}
```
<!--
{
  "type": "#page.annotation",
  "description": "programControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


