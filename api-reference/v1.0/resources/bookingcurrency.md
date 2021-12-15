---
title: bookingCurrency 资源类型
description: 表示 bookingBusiness 支持的货币货币。
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 47cddfdf3a127941414ceaccba500d4bba357aa3
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525021"
---
# <a name="bookingcurrency-resource-type"></a>bookingCurrency 资源类型

命名空间：microsoft.graph

表示由 [bookingBusiness 支持的货币货币](bookingbusiness.md)。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 bookingCurrencies](../api/bookingcurrency-list.md) | [bookingCurrency](bookingcurrency.md) 集合 |获取可用于 Microsoft **Bookings 业务的 bookingCurrency** 对象列表。|
|[获取 bookingCurrency](../api/bookingcurrency-get.md) | [bookingCurrency](bookingcurrency.md) |获取 **bookingCurrency 对象** 的属性。|


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 基于 [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html)的 3 字符货币代码。 例如，美元的货币代码为 USD，澳大利亚元为 AUD。 只读。|
|符号|String| 货币符号。 例如，美元和澳大利亚元的货币符号为 $。  |

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingCurrency"
}-->

```json
{
  "id": "String (identifier)",
  "symbol": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingCurrency resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


