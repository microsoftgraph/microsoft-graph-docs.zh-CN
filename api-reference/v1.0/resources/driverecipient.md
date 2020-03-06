---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.prod: sharepoint
description: DriveRecipient 资源表示用户、组或其他收件人使用 invite 操作进行共享。
doc_type: resourcePageType
ms.openlocfilehash: d1b123c897791dff5bd6c42eb9e4b030e83e1d5c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531534"
---
# <a name="driverecipient-resource"></a>DriveRecipient 资源

命名空间：microsoft.graph

**DriveRecipient** 资源表示用户、组或其他收件人使用 [invite](../api/driveitem-invite.md) 操作进行共享。

## <a name="json-representation"></a>JSON 表示形式

<!-- { 
  "blockType": "resource", 
  "@odata.type": "microsoft.graph.driveRecipient", 
  "optionalProperties": ["alias", "objectId", "email"] } -->
```json
{
  "email": "string",
  "alias": "string",
  "objectId": "string",
}
```

## <a name="properties"></a>属性
收件人资源具有以下属性。

| 属性名称 | 类型   | 说明                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| email         | String | 收件人的电子邮件地址，前提是收件人有关联的电子邮件地址。                  |
| 别名         | 字符串 | Domain 对象的别名，适于电子邮件地址不可用的情况（例如，安全组）。 |
| objectId      | String | 目录中收件人的唯一标识符。                                               |

## <a name="remarks"></a>注解

当使用 [邀请](../api/driveitem-invite.md) 添加权限时，DriveRecipient 可以指定**电子邮件**、**别名**或**对象 ID**。这些值中只有一个是必需的。

<!-- {
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients"
} -->
