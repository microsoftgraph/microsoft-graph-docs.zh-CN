---
title: keyCredentialConfiguration 资源类型
description: 用于配置密钥凭据限制、maxLifetime 和强制执行日期的密钥凭据配置复杂类型
ms.localizationpriority: medium
author: madansr7
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 05fc7bab3a5073032ca3d27fd63424ff5b6fea56
ms.sourcegitcommit: 42e0e15ff90815e0126c34b928405486cfb1ed86
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/17/2021
ms.locfileid: "61044783"
---
# <a name="keycredentialconfiguration-resource-type"></a>keyCredentialConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含用于配置限制（如限制密钥密钥生存期）的属性的密钥凭据配置对象。

## <a name="properties"></a>属性

| 属性                            | 类型                                                                               | 说明                                                                                                                                                                                                                                                                                   |
| :---------------------------------- | :--------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| restrictionType                     | appKeyCredentialRestrictionType | 要应用的限制的类型。 可能的值是 `asymmetricKeyLifetime` `unknownFutureValue` 、。 每个 restrictionType 值只能用于每个策略一次。                                                                                                                        |
| maxLifeTime                         | 期限                                                                           |可用于作为密钥创建日期（密钥有效）的最长持续时间（以天、小时、分钟或秒表示）的值。  以 ISO 8601 格式定义持续时间。 例如， `P4DT12H30M5S` 表示持续时间为四天、十二小时、三十分钟和五秒。 当 **restrictionType** 设置为 时，此属性是必需的 `keyLifetime` 。 |
| restrictForAppsCreatedAfterDateTime | DateTimeOffset                                                                     | 对指定日期当天或之后创建的所有应用强制执行策略的时间戳。 对于现有应用程序，强制执行日期将回到日期。 若要应用于所有应用程序，而不考虑其创建日期，此属性为 `null` 。 可为空。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyCredentialConfiguration"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.keyCredentialConfiguration",
  "restrictionType": {
    "@odata.type": "microsoft.graph.appKeyCredentialRestrictionType"
  },
  "maxLifetime": "String (duration)",
  "restrictForAppsCreatedAfterDateTime": "DateTimeOffset"
}
```
