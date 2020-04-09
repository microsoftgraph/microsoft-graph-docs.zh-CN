---
title: onPremisesProvisioningError 资源类型
description: 表示在将本地目录同步到 Azure Active Directory 时，用户、组或组织联系人实体的目录同步错误。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: japere
ms.openlocfilehash: 6765f23f6d3a5cc5b31363506f63ed6949810646
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/09/2020
ms.locfileid: "43200059"
---
# <a name="onpremisesprovisioningerror-resource-type"></a>onPremisesProvisioningError 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在将本地目录同步到 Azure Active Directory 时，[用户](user.md)、[组](group.md)或[组织联系人](orgcontact.md)实体的目录同步错误。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|“类别”|字符串| 设置错误的类别。 注意：目前，只有一个可能的值。 可能的值： *PropertyConflict* -指示属性值不是唯一的。 其他对象包含相同的属性值。 |
|occurredDateTime|DateTimeOffset| 发生错误的日期和时间。 |
|propertyCausingError|字符串| 导致错误的目录属性的名称。 当前可能的值： *UserPrincipalName*或*ProxyAddress* |
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
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
