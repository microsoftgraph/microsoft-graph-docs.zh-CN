---
title: educationRoot 资源类型
description: '`/education` 命名空间公开特定于教育部门的功能。 '
author: mmast-msft
ms.openlocfilehash: 2a9eac02552e62e7bfb889e9e87efe47fa5f88f9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307432"
---
# <a name="educationroot-resource-type"></a>educationRoot 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

`/education` 命名空间公开特定于教育部门的功能。 `/education` 命名空间中的一些对象可在 Microsoft Graph 的其他部分中找到（例如，[users](user.md)）。 教育命名空间提供有关这些对象特定于教育的属性和功能。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Create educationClass](../api/educationroot-post-classes.md) |[educationClass](educationclass.md)| 通过发布到 classes 集合创建新的 **educationClass**。|
|[List classes](../api/educationroot-list-classes.md) |[educationClass](educationclass.md) 集合| 获取 **educationClass** 对象集合。|
|[Create educationSchool](../api/educationroot-post-schools.md) |[educationSchool](educationschool.md)| 通过发布到 schools 集合创建新的 **educationSchool**。|
|[List schools](../api/educationroot-list-schools.md) |[educationSchool](educationschool.md) 集合| 获取 **educationSchool** 对象集合。|
|[Create educationUser](../api/educationroot-post-users.md) |[educationUser](educationuser.md)| 通过发布到 users 集合创建新的 **educationUser**。|
|[List users](../api/educationroot-list-users.md) |[educationUser](educationuser.md) 集合| 获取 **educationUser** 对象集合。|

## <a name="properties"></a>属性
无。

## <a name="relationships"></a>Relationships
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|classes|[educationClass](educationclass.md) 集合| 只读。可为 NULL。|
|me|[educationUser](educationuser.md)| 只读。可为 NULL。|
|schools|[educationSchool](educationschool.md) 集合| 只读。可为 NULL。|
|users|[educationUser](educationuser.md) 集合| 只读。可为 NULL。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->