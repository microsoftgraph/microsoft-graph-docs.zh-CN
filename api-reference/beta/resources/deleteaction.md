---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: DeleteAction
ms.openlocfilehash: 041552f88561981338fa2ea5719d5af102fb3574
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043981"
---
# <a name="deleteaction-resource-type"></a>DeleteAction 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

[**itemActivity**][activity] 上存在 **DeleteAction** 资源指示活动删除了一个项。

[activity]: itemactivity.md

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.deleteAction"
}-->

```json
{
  "name": "string",
  "objectType": "File | Folder"
}
```

## <a name="properties"></a>属性

| 属性名称 | 类型   | 说明
|:--------------|:-------|:----------------------------------------------------
| name          | string | 已删除的项的名称。
| objectType    | string | `File`或`Folder`，具体取决于已删除的项目的类型。

## <a name="remarks"></a>注解

项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。

<!-- {
  "type": "#page.annotation",
  "description": "The DeleteAction object provides information about the deletion of an item.",
  "keywords": "activities,activity,action,delete,deletion",
  "section": "documentation",
  "tocPath": "Resources/DeleteAction"
} -->
