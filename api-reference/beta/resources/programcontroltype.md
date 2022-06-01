---
title: 'programControlType 资源类型 (已弃用) '
description: '在 Azure AD 访问评审功能中，将控件与程序关联时使用程序控件类型，以指示控件用于的访问评审类型。  '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 2dcb4c5e00b4c3b5ea0cf9283dadaa9b2c89cd12
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819736"
---
# <a name="programcontroltype-resource-type-deprecated"></a>programControlType 资源类型 (已弃用) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

在 Azure AD [访问评审](accessreviews-root.md) 功能中，将控件与程序关联时使用程序控件类型，以指示控件用于的访问评审类型。  

当全局管理员载入租户以使用访问评审功能时，将自动生成程序控制类型对象。  无法创建其他程序控制类型。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 programControlTypes](../api/programcontroltype-list.md) | [programControlType](programcontroltype.md) 集合| 列出程序控制类型。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| id                     |String                | 程序控件类型的功能分配标识符                                      |
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


