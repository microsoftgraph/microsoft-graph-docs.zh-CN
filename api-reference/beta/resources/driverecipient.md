---
author: JeremyKelley
description: driveRecipient 资源表示使用 invite 操作要共享的人、组或其他收件人。
ms.date: 09/10/2017
title: DriveRecipient
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 1b7b666e520af98fd6fae193b770357a7813504e
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2022
ms.locfileid: "63722575"
---
# <a name="driverecipient-resource"></a>driveRecipient 资源

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示使用 invite 操作共享驱动器项目的人、组[或其他收件人。](../api/driveitem-invite.md)

使用 [invite](../api/driveitem-invite.md) 添加权限时，**driveRecipient** 对象可以指定 **收件人** 的电子邮件、别名或 **objectId**。 
只需要其中一个值;不接受多个值。

## <a name="properties"></a>属性

收件人资源具有以下属性。

| 属性 | 类型   | 说明                                                                                             |
| :------- | :----- | :------------------------------------------------------------------------------------------------------ |
| email    | String | 收件人的电子邮件地址，前提是收件人有关联的电子邮件地址。                  |
| 别名    | String | Domain 对象的别名，适于电子邮件地址不可用的情况（例如，安全组）。 |
| objectId | String | 目录中收件人的唯一标识符。                                               |

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

<!--
{
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients",
  "suppressions": []
}
-->
