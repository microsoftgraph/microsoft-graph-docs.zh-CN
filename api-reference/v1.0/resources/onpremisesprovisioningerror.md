---
title: onPremisesProvisioningError 资源类型
description: 同步到 Azure Active Directory 的内部部署目录时，表示为用户和组的实体的目录同步错误。
localization_priority: Normal
ms.openlocfilehash: c8989a78dfb60a6c7c25a66a9f1e619dcbdca15d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830665"
---
# <a name="onpremisesprovisioningerror-resource-type"></a>onPremisesProvisioningError 资源类型

时同步部署到 Azure Active Directory 目录，则表示[用户](user.md)和[组](group.md)实体的目录同步错误。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|category|String| 设置错误的类别。 注意： 当前，没有只有一个可能的值。 可能的值： *PropertyConflict* -指示属性值不唯一。 其他对象包含的属性相同的值。 |
|occurredDateTime|DateTimeOffset| 日期和时间发生错误。 |
|propertyCausingError|字符串| 导致此错误的目录属性的名称。 当前的可能值： *UserPrincipalName*或*ProxyAddress* |
|值|字符串| 导致错误属性的值。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesProvisioningError"
}-->

```json
{
  "category": "String",
  "occurredDateTime": "String (timestamp)",
  "propertyCausingError": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
