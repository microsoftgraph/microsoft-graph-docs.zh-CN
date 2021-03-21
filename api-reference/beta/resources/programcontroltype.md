---
title: programControlType 资源类型
description: '在 Azure AD 访问评审功能中，将控件关联到程序时，会使用程序控件类型来指示控件所针对的访问评审类型。  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 58c9ee3ade6e3969de9653f54c5181a66f087ea5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960360"
---
# <a name="programcontroltype-resource-type"></a>programControlType 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 Azure [AD](accessreviews-root.md) 访问评审功能中，将控件关联到程序时，会使用程序控件类型来指示控件所针对的访问评审类型。  

当全局管理员载入租户以使用访问评审功能时，将自动生成程序控制类型对象。  无法创建其他程序控制类型。


## <a name="methods"></a>Methods

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 programControlTypes](../api/programcontroltype-list.md) | [programControlType](programcontroltype.md) 集合| 列出程序控件类型。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| id                     |String                | 程序控件类型的功能分配的标识符                                      |
| displayName            |String                | 程序控件类型的名称                                                             |


## <a name="relationships"></a>关系

无。


## <a name="see-also"></a>另请参阅

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[创建 programControl](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   将 programControl 添加到程序。|


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

<!--
{
  "type": "#page.annotation",
  "description": "programControlType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


