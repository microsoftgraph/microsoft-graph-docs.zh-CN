---
title: passwordCredential 资源类型
description: 包含与应用程序或服务主体相关联的密码凭据。 ServicePrincipal 实体和 application 实体的**passwordCredentials**属性是**passwordCredential**的集合。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 0067b993cfc7d9708673bf25b20ecc054bff7925
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534078"
---
# <a name="passwordcredential-resource-type"></a>passwordCredential 资源类型

命名空间：microsoft.graph

表示与应用程序或服务主体相关联的密码凭据。 [应用程序](application.md)的**passwordCredentials**属性 <!--and [servicePrincipal](serviceprincipal.md) entitites--> entity 是**passwordCredential**对象的集合。

> [!IMPORTANT]
> 不支持使用 POST 或 PATCH 设置**passwordCredential** 。 使用 addPassword 和 removePassword 方法更新应用程序的密码<!--or a servicePrincipal-->:
>
> - [应用程序： addPassword](../api/application-addpassword.md)
> - [应用程序： removePassword](../api/application-removepassword.md)
<!--
> - [servicePrincipal: addPassword](../api/serviceprincipal-addpassword.md)
> - [servicePrincipal: removePassword](../api/serviceprincipal-removepassword.md)
-->

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| customKeyIdentifier | Binary | 请勿使用。 |
| displayName | String | 密码的友好名称。 可选。 |
| endDateTime | DateTimeOffset | 密码过期的日期和时间，使用 ISO 8601 格式表示，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。 可选。 |
| 提示 | 字符串 | 包含密码的前三个字符。 只读。 |
| keyId | Guid | 密码的唯一标识符。 |
| secretText | 字符串 | 只读;包含由 Azure AD 生成的强密码，其长度为16-64 个字符。 生成的密码值仅在初始 POST 请求过程中返回到[addPassword](../api/application-addpassword.md)。 将来无法检索此密码。 |
| startDateTime | DateTimeOffset | 密码生效的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。 可选。 |

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
  "keyId": "Guid",
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
