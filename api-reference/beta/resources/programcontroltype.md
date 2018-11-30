---
title: programControlType 资源类型
description: '在 Azure AD 中访问审阅功能，为关联到程序，以指示类型的访问审阅控件控件时使用的程序控件类型。  '
ms.openlocfilehash: 8fc406648d8f8c943920507a5734f47d2add1b4c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045454"
---
# <a name="programcontroltype-resource-type"></a>programControlType 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

在 Azure AD[访问审阅](accessreviews-root.md)功能中的程序控件类型用于将控件与程序相关联时指示的访问查看该控件的类型。  

全局管理员 onboards 租户用于访问审阅功能时，将自动生成的程序控件类型对象。  可以不创建任何其他程序控件类型。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列表 programControlTypes](../api/programcontroltype-list.md) | [programControlType](programcontroltype.md)集合| 列出程序控件类型。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| `id`                     |`String`                | 程序控件类型的功能指派的标识符                                      |
| `displayName`            |`String`                | 程序控件类型的名称                                                             |


## <a name="relationships"></a>Relationships

无。


## <a name="see-also"></a>另请参阅

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[创建 programControl](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   添加到程序 programControl。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programControlType"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string"
}

```

<!-- {
  "type": "#page.annotation",
  "description": "programControlType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
