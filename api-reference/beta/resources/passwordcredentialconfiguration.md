---
title: passwordCredentialConfiguration 资源类型
description: 用于配置密码凭据限制、maxLifetime 和强制执行日期的密码凭据配置复杂类型
author: madansr7
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: fb7d9728100d15fcbc485f5825cafab5b5726973
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337514"
---
# <a name="passwordcredentialconfiguration-resource-type"></a>passwordCredentialConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含用于配置限制（如阻止或限制密码密码生存期）的属性的密码凭据配置对象。

## <a name="properties"></a>属性

| 属性                            | 类型                         | 说明                                                                                                                                                                                                                                                                                                                                                   |
| :---------------------------------- | :--------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| restrictionType                     | appCredentialRestrictionType | 要应用的限制的类型。 可能的值是：、`passwordAddition`、`passwordLifetime`、`symmetricKeyAddition``symmetricKeyLifetime`、`customPasswordAddition`、`unknownFutureValue`。 每个 restrictionType 值只能用于每个策略一次。                                                                                        |
| maxLifeTime                         | 期限                     | 可以用作设置密码过期时间的最大数目的值（以天、小时、分钟或秒表示）。 以 ISO 8601 格式定义持续时间。 例如，"P4DT12H30M5S"表示持续时间为四天、十二小时、三十分钟和五秒。 当限制类型设置为 时，此属性是必需的 `passwordLifetime`。 |
| restrictForAppsCreatedAfterDateTime | DateTimeOffset               | 强制执行在强制执行日期或之后创建的应用的策略。 对于现有应用程序，将备份强制执行日期。 若要应用于所有应用程序，此日期为 `null`。                                                                                                                                               |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.passwordCredentialConfiguration"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.passwordCredentialConfiguration",
  "restrictionType": {
    "@odata.type": "microsoft.graph.appCredentialRestrictionType"
  },
  "maxLifetime": "String (duration)",
  "restrictForAppsCreatedAfterDateTime": "DateTimeOffset"
}
```
