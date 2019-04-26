---
title: programControlType 资源类型
description: '在 Azure AD access 评论功能中, 将控件与程序关联时使用程序控件类型, 以指示控件所针对的访问评审的类型。  '
localization_priority: Normal
ms.openlocfilehash: 489fa6e5cac31165fec9f7ce9939d58fa84cb1ab
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344042"
---
# <a name="programcontroltype-resource-type"></a>programControlType 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 Azure AD [access 评论](accessreviews-root.md)功能中, 将控件与程序关联时使用程序控件类型, 以指示控件所针对的访问评审的类型。  

当全局管理员 onboards 租户使用访问评论功能时, 将自动生成程序控制类型对象。  无法创建其他程序控件类型。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 programControlTypes](../api/programcontroltype-list.md) | [programControlType](programcontroltype.md)集合| 列出程序控制类型。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| `id`                     |`String`                | 为程序控件类型分配的功能的标识符                                      |
| `displayName`            |`String`                | 程序控件类型的名称                                                             |


## <a name="relationships"></a>Relationships

无。


## <a name="see-also"></a>另请参阅

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[创建 programControl](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   将 programControl 添加到程序中。|


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
