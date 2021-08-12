---
title: onPremisesProvisioningError 资源类型
description: 表示将本地目录同步到本地目录时用户组和联系人资源的目录Azure Active Directory。
localization_priority: Normal
author: japere
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 7c3e50469b9625c62d587f75fa778a3408699952eda4a204b8aaccbb73a80e2f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54216670"
---
# <a name="onpremisesprovisioningerror-resource-type"></a>onPremisesProvisioningError 资源类型

命名空间：microsoft.graph

表示将本地目录同步到本地[目录时](user.md)用户、[组](group.md)和[orgContact](orgcontact.md)资源的目录Azure Active Directory。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|“类别”|String| 设置错误的类别。 注意：目前，只有一个可能的值。 可能的值 *：PropertyConflict* - 指示属性值不唯一。 其他对象包含与属性相同的值。 |
|occurredDateTime|DateTimeOffset| 发生错误的日期和时间。 |
|propertyCausingError|String| 导致错误的目录属性的名称。 当前可能的值 *：UserPrincipalName* 或 *ProxyAddress* |
|value|String| 导致错误的属性的值。 |

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

