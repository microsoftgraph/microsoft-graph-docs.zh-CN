---
title: passwordCredential 资源类型
description: 包含与应用程序或服务主体关联的密码凭据。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 4a6a783cc088585aeb50afa9984d1dbf30e629ae
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2022
ms.locfileid: "62855183"
---
# <a name="passwordcredential-resource-type"></a>passwordCredential 资源类型

命名空间：microsoft.graph

表示与应用程序或服务主体关联的密码凭据。 **应用程序的 passwordCredentials** [属性](application.md) <!--and [servicePrincipal](serviceprincipal.md) entitites--> entity 是 **passwordCredential 对象** 的集合。

> [!IMPORTANT]
> 不支持使用 POST 或 PATCH 设置 **passwordCredential** 属性。 使用以下 addPassword 和 removePassword 方法更新应用程序或 servicePrincipal 的密码：
>
> - [application： addPassword](../api/application-addpassword.md)
> - [application： removePassword](../api/application-removepassword.md)
> - [servicePrincipal：addPassword](../api/serviceprincipal-addpassword.md)
> - [servicePrincipal：removePassword](../api/serviceprincipal-removepassword.md)

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| customKeyIdentifier | Binary | 请勿使用。 |
| displayName | String | 密码的友好名称。 可选。 |
| endDateTime | DateTimeOffset | 密码过期的日期和时间使用 ISO 8601 格式表示，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 可选。 |
| hint | String | 包含密码的前三个字符。 只读。 |
| keyId | GUID | 密码的唯一标识符。 |
| secretText | String | 只读;包含由 Azure AD生成的强密码，长度为 16-64 个字符。 生成的密码值仅在初始 POST 请求 [addPassword 期间返回](../api/application-addpassword.md)。 将来无法检索此密码。 |
| startDateTime | DateTimeOffset | 密码生效的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 可选。 |

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


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordCredential",
  "baseType": null
}-->

```json
{
  "customKeyIdentifier": "Binary",
  "displayName": "String",
  "endDateTime": "String (timestamp)",
  "hint": "String",
  "keyId": "GUID",
  "secretText": "String",
  "startDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

