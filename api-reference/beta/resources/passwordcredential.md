---
title: passwordCredential 资源类型
description: 包含与应用程序或服务主体相关联的密码凭据。 servicePrincipal 实体和 application 实体的**passwordCredentials**属性是**passwordCredential**的集合。
localization_priority: Normal
ms.openlocfilehash: f00deb42dcc24fc6d8218239d5d807ee21b2f7c3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345004"
---
# <a name="passwordcredential-resource-type"></a>passwordCredential 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含与应用程序或服务主体相关联的密码凭据。 [servicePrincipal](serviceprincipal.md)实体和[application](application.md)实体的**passwordCredentials**属性是**passwordCredential**的集合。


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "secretText": "string",
  "hint": "string"
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|customKeyIdentifier|Binary|            |
|endDateTime|DateTimeOffset|密码过期的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息, 并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|keyId|Guid|            |
|startDateTime|DateTimeOffset|密码生效的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息, 并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|secretText|String| 密码长度必须为16-64 个字符 |
|提示|String|  |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
