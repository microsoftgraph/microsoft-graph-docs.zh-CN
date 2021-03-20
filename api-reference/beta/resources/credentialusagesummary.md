---
title: credentialUsageSummary 资源类型
description: 表示组织中使用自助服务密码重置功能的用户数的当前状态。
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 9db31a0d0397f1394a342fb52796a1bec37bae36
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941822"
---
# <a name="credentialusagesummary-resource-type"></a>credentialUsageSummary 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示组织中使用自助服务密码重置功能的用户数的当前状态。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [getCredentialUsageSummary](../api/reportroot-getcredentialusagesummary.md) | credentialUsageSummary | 读取 credentialUsageSummary 对象的属性和关系。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| authMethod | usageAuthMethod | 表示用户使用的身份验证方法。 可能的值是：、 (仅用于自助服务密码重置 `email` `mobileSMS` `mobileCall` `officePhone` `securityQuestion`) 、 (仅在注册 `appNotification` `appCode` `alternateMobileCall` `fido` `appPassword` `unknownFutureValue`) 、。 |
| failureActivityCount | Int64 | 提供失败的重置或注册数据计数。 |
| 功能 | featureType | 定义要报告的功能。 可取值为：`registration`、`reset`、`unknownFutureValue`。 |
| id | String | 活动的唯一标识符。 只读。 |
| successfulActivityCount | Int64 | 提供成功注册或重置的计数。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUsageSummary",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "feature":"string",
  "successfulActivityCount":"Int64",
  "failureActivityCount": "Int64",
  "authMethod": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "credentialUsageSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

