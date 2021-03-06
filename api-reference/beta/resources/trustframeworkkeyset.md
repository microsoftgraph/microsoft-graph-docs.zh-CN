---
title: trustFrameworkKeySet 资源类型
description: 表示信任框架键集/策略密钥。
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4bd20bd3b9df4656a3bbc73a52511d64ad463bf5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442766"
---
# <a name="trustframeworkkeyset-resource-type"></a>trustFrameworkKeySet 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示信任框架键集/策略密钥。 标识体验框架存储可在策略中使用的密钥。 密钥可以是密码、证书或其他文件。 在门户中，这些实体显示为 `Policy keys` 。 标识体验框架使用 JSON Web 密钥 (JWK) JWK 标准。 此实体遵循 [RFC 7517 第 5 节中指定的格式](https://tools.ietf.org/html/rfc7517#section-5)。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
| [List](../api/trustframework-list-keysets.md) | [trustFrameworkKeySet](trustframeworkkeyset.md) 集合 | 列出 trustFrameworkKeySets。 |
| [创建](../api/trustframework-post-keysets.md) | [trustFrameworkKeySet](trustframeworkkeyset.md) | 创建 trustFrameworkKeySet。 |
| [获取](../api/trustframeworkkeyset-get.md) | [trustFrameworkKeySet](trustframeworkkeyset.md) | 读取 trustFrameworkKeySet 对象的属性和关系。 |
| [更新](../api/trustframeworkkeyset-update.md) | [trustFrameworkKeySet](trustframeworkkeyset.md) | 更新 trustFrameworkKeySet 对象。 |
| [删除](../api/trustframeworkkeyset-delete.md) | 无 | 删除 trustFrameworkKeySet 对象。 |
|[生成密钥](../api/trustframeworkkeyset-generatekey.md)|[trustFrameworkKey](trustframeworkkey.md)| 在键集内生成键。 |
|[获取活动键](../api/trustframeworkkeyset-getactivekey.md)|[trustFrameworkKey](trustframeworkkey.md)| 获取键集中的当前活动键。 |
|[上载证书](../api/trustframeworkkeyset-uploadcertificate.md)|[trustFrameworkKey](trustframeworkkey.md)| 上载 X.509 证书。 |
|[上载 PKCS12](../api/trustframeworkkeyset-uploadpkcs12.md)|[trustFrameworkKey](trustframeworkkey.md)| 上载 PKCS12 格式证书。 |
|[上传密码](../api/trustframeworkkeyset-uploadsecret.md)|[trustFrameworkKey](trustframeworkkey.md)| 上载基于字符串的机密。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| trustframework 键集的唯一标识符 |
|键|[trustFrameworkKey](trustframeworkkey.md) 集合| 键的集合。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.trustFrameworkKeySet",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "keys": [{"@odata.type": "microsoft.graph.trustFrameworkKey"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


