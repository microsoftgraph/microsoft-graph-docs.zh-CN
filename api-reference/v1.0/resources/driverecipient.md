---
author: JeremyKelley
ms.date: 09/10/2017
title: DriveRecipient
ms.localizationpriority: medium
ms.prod: sharepoint
description: driveRecipient 资源表示使用 invite 操作要共享的人、组或其他收件人。
doc_type: resourcePageType
ms.openlocfilehash: 4788b02e0ec52965475745a4e234beaaf6b2910e
ms.sourcegitcommit: 94dc71a6d4fbdc46f2681a1add13416bc9b4a6e9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2021
ms.locfileid: "60115387"
---
# <a name="driverecipient-resource"></a>driveRecipient 资源

命名空间：microsoft.graph

表示使用 invite 操作共享驱动器项目的人、组[或其他收件人。](../api/driveitem-invite.md)

使用 [invite](../api/driveitem-invite.md)添加权限时 **，driveRecipient** 对象将指定 **收件人** 的电子邮件、**别名** 或 **objectId。**
只需要其中一个值;不接受多个值。

## <a name="properties"></a>属性
收件人资源具有以下属性。

| 属性名称 | 类型   | 说明                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| email         | String | 收件人的电子邮件地址，前提是收件人有关联的电子邮件地址。                  |
| 别名         | String | Domain 对象的别名，适于电子邮件地址不可用的情况（例如，安全组）。 |
| objectId      | String | 目录中收件人的唯一标识符。                                               |

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

<!-- {
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients"
} -->

