---
title: keyCredential 资源类型
description: 包含与应用程序或服务主体关联的密钥凭据。 application 和 servicePrincipal 实体的 **keyCredentials** 属性是 **keyCredential 的集合**。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: madansr7
ms.openlocfilehash: f0c92a613c234fccfd757d0144eefdb51a0ec316
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2022
ms.locfileid: "62804372"
---
# <a name="keycredential-resource-type"></a>keyCredential 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含与应用程序或服务主体关联的密钥凭据。 application 和 [servicePrincipal](serviceprincipal.md) 实体的 [](application.md) **keyCredentials** 属性是 **keyCredential 的集合**。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|customKeyIdentifier|Binary| 自定义密钥标识符 |
| displayName | 字符串 | 密钥的友好名称。 可选。 |
|endDateTime|DateTimeOffset|凭据过期的日期和时间。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|key|二进制| 密钥凭据的值。 应为 Base64 编码的值。 仅对 `$select` 单个对象（ `GET applications/{applicationId}?$select=keyCredentials` 即 或 `GET servicePrincipals/{servicePrincipalId}?$select=keyCredentials`）返回 ;否则，始终为 `null`。 |
|keyId|Guid|密钥的唯一标识符。|
|startDateTime|DateTimeOffset|凭据生效的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|type|字符串|密钥凭据的类型;例如，。 `Symmetric``AsymmetricX509Cert`|
|usage|字符串|一个描述密钥的用途的字符串;例如， `Verify`。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyCredential"
}-->

```json
{
  "@odata.type": "#microsoft.graph.keyCredential",
  "customKeyIdentifier": "Binary",
  "displayName": "String",
  "endDateTime": "String (timestamp)",
  "key": "Binary",
  "keyId": "Guid",
  "startDateTime": "String (timestamp)",
  "type": "String",
  "usage": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "keyCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


