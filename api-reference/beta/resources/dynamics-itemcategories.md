---
title: itemCategories 资源类型
description: Dynamics 365 Business Central 中的项类别。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 18017c580637bb53a70b5f7a331ff7be1dc7a07c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972920"
---
# <a name="itemcategories-resource-type"></a>itemCategories 资源类型
代表 Dynamics 365 Business Central 中的大量项目的类别。

## <a name="methods"></a>方法

| 方法                                                          | 返回类型  |说明             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[获取 itemCategories](../api/dynamics-itemcategories-get.md)      |itemCategories|获取项目类别。   |
|[Post itemCategories](../api/dynamics-create-itemcategories.md)  |itemCategories|创建项类别。|
|[修补程序 itemCategories](../api/dynamics-itemcategories-update.md) |itemCategories|更新项目类别。|
|[删除 itemCategories](../api/dynamics-itemcategories-delete.md)|无          |删除项目类别。|

## <a name="properties"></a>属性
| 属性           | 类型   |说明                                     |
|:-------------------|:-------|:-----------------------------------------------|
|id                  |GUID    |ItemCategory 的唯一 ID。 不可编辑。|
|code                |string  |ItemCategory 代码。                          |
|displayName         |string  |ItemCategories 显示名称。                |
|lastModifiedDateTime|datetime|上次修改 itemCategory 的日期/时间。 只读。|  


## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式

下面是 itemCategories 的 JSON 表示形式。

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}
```

