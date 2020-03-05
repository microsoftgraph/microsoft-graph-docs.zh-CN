---
title: 复杂类型 JSON
description: JSON for Dynamics 365 Business Central 中的复杂数据类型。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 59aa494c8396d1370dc588b459c7b76f1614e9cc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42504984"
---
# <a name="complex-types-json"></a>复杂类型 JSON

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

这些是 Dynamics 365 Business Central 中的各种复杂类型。 您可以在使用这些复杂类型的各种不同方法中查看这些复杂类型的用法。

## <a name="postal-address"></a>邮政地址

代表 Dynamics 365 Business Central 中的邮政地址复杂类型。

### <a name="properties"></a>属性
| 属性     | 类型       |说明             |
|:-------------|:---------|:-----------------------|
|street        |string    |邮政地址街道。  |
|城市          |string    |邮政地址（城市）。    |
|state         |string    |邮政地址状态。   |
|countryLetterCode|string |通信地址国家/地区字母代码（两个字符的单词）|
|postalCode    |string    |邮政地址发布代码|

```json
"PostalAddress" 
{ 
"street": "string",
"city": "string", 
"state": "string", 
"countryLetterCode": "string", 
"postalCode": "string" 
} 
 ```

