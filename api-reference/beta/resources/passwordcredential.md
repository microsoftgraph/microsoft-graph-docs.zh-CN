---
title: passwordCredential 资源类型
description: 包含与应用程序或服务主体密码凭据。 **PasswordCredentials**属性和应用程序实体的 servicePrincipal 实体是**passwordCredential**的集合。
ms.openlocfilehash: 79d3f76606533cf639f52ed22cd93f353e18e977
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041559"
---
# <a name="passwordcredential-resource-type"></a>passwordCredential 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

包含与应用程序或服务主体密码凭据。 **PasswordCredentials**属性和[应用程序](application.md)实体的[servicePrincipal](serviceprincipal.md)实体是**passwordCredential**的集合。


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
|customKeyIdentifier|二进制数|            |
|endDateTime|DateTimeOffset|过期日期和时间的密码。时间戳类型表示使用 ISO 8601 格式的日期和时间信息且始终在 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|密钥 id 为|Guid|            |
|startDateTime|DateTimeOffset|日期和时间的密码将成为有效。时间戳类型表示使用 ISO 8601 格式的日期和时间信息且始终在 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|secretText|字符串| 密码必须为 16-64 个字符的长度 |
|提示|String|  |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
