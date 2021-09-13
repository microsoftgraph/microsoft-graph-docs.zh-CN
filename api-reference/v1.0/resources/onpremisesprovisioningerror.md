---
title: onPremisesProvisioningError 资源类型
description: 表示将本地目录同步到本地目录时用户组和联系人资源的目录Azure Active Directory。
ms.localizationpriority: medium
author: japere
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 9f95b454b37913c407e949cc76cd01e48299e785
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59071992"
---
# <a name="onpremisesprovisioningerror-resource-type"></a>onPremisesProvisioningError 资源类型

命名空间：microsoft.graph

表示用户、组和[orgContact](orgcontact.md)资源的目录同步错误（将本地目录同步到 Azure Active Directory）。 [](user.md) [](group.md)

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

