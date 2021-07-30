---
title: passwordCredentialConfiguration 资源类型
description: 用于配置密码凭据限制、maxLifetime 和强制执行日期的密码凭据配置复杂类型
author: madansr7
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 8a67dfd1bf6ee717f279cb27bf08f819daba1645
ms.sourcegitcommit: b711aed8acc18512cf6591f4108ed5ddf05b649d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2021
ms.locfileid: "53660349"
---
# <a name="passwordcredentialconfiguration-resource-type"></a>passwordCredentialConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含用于配置限制（如阻止或限制密码密码生存期）的属性的密码凭据配置对象。

## <a name="properties"></a>属性

| 属性                            | 类型                                                                               | 说明                                                                                                                                                                                                                                                                                   |
| :---------------------------------- | :--------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| restrictionType                     | appCredentialRestrictionType | 要应用的限制的类型。 可能的值为 `passwordAddition` 或 `passwordLifetime`。 每个 restrictionType 值只能用于每个策略一次。                                                                                                                        |
| maxLifeTime                         | 期限                                                                           | 可以用作设置密码过期时间的最大数目的值（以天、小时、分钟或秒表示）。 例如，"P4DT12H30M5S"表示持续时间为四天、十二小时、三十分钟和五秒。 当限制类型设置为 时，此属性是必需的 `passwordLifetime` 。 |
| restrictForAppsCreatedAfterDateTime | DateTimeOffset                                                                     | 强制执行在强制执行日期或之后创建的应用的策略。 对于现有应用程序，强制执行日期将回到日期。 若要应用于所有应用程序，强制日期/时间为 null。                                                                               |

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
