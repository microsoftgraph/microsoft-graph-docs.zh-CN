---
title: keyCredential 资源类型
description: 包含与应用程序或服务主体关键凭据。 应用程序和 servicePrincipal 实体的**keyCredentials**属性是**keyCredential**的集合。
localization_priority: Normal
ms.openlocfilehash: 0319568dad271f13b396d2f75a71839e85c96c40
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851560"
---
# <a name="keycredential-resource-type"></a>keyCredential 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

包含与应用程序或服务主体关键凭据。 [应用程序](application.md)和[servicePrincipal](serviceprincipal.md)实体的**keyCredentials**属性是**keyCredential**的集合。


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
  "customKeyIdentifier": "binary",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "type": "string",
  "usage": "string",
  "key": "binary"
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|customKeyIdentifier|Binary| 自定义的密钥标识符 |
|endDateTime|DateTimeOffset|过期日期和时间的凭据。时间戳类型表示使用 ISO 8601 格式的日期和时间信息且始终在 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|密钥 id 为|Guid|唯一标识符 (GUID) 键。|
|startDateTime|DateTimeOffset|日期和时间凭据生效。时间戳类型表示使用 ISO 8601 格式的日期和时间信息且始终在 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|type|字符串|类型的关键凭据;例如，"对称"。|
|使用情况|字符串|描述其密钥可用于; 用途的字符串例如，"验证"。|
|key|二进制|            |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "keyCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
