---
title: credentialUsageSummary 资源类型
description: 表示组织中的多少用户使用自助密码重置功能的当前状态。
localization_priority: Normal
author: khotz
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 736575ba8958a45cad76f7142967c2a629b0732a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43458024"
---
# <a name="credentialusagesummary-resource-type"></a>credentialUsageSummary 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示组织中的多少用户使用自助密码重置功能的当前状态。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [getCredentialUsageSummary](../api/reportroot-getcredentialusagesummary.md) | credentialUsageSummary | 读取 credentialUsageSummary 对象的属性和关系。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| authMethod | string | 表示用户使用的身份验证方法。 可能的值是`email`： `mobileSMS`、 `mobileCall`、 `officePhone`、 `securityQuestion` 、（仅用于自助密码重置）、 `appNotification` `appCode`、和`alternateMobileCall` （仅支持注册）。 |
| failureActivityCount | Int64 | 提供失败重置或注册数据的计数。 |
| 功能 | string | 定义要报告的功能。 可能的值为`registration` ： `reset`和。 |
| id | String | 活动的唯一标识符。 只读。 |
| successfulActivityCount | Int64 | 提供成功注册或重置的次数。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUsageSummary",
  "baseType": "",
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