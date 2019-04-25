---
title: 复杂类型 JSON
description: JSON for Dynamics 365 Business Central 中的复杂数据类型。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4fc4d4f53014f5b8c656cd069cadf7b19190e0f0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543160"
---
# <a name="complex-types-json"></a>复杂类型 JSON
这些是 Dynamics 365 Business Central 中的各种复杂类型。 您可以在使用这些复杂类型的各种不同方法中查看这些复杂类型的用法。

## <a name="postal-address"></a>邮政地址

代表 Dynamics 365 Business Central 中的邮政地址复杂类型。

### <a name="properties"></a>属性
| 属性     | 类型       |说明             |
|:-------------|:---------|:-----------------------|
|street        |string    |邮政地址街道。  |
|city          |string    |邮政地址 (城市)。    |
|state         |string    |邮政地址状态。   |
|countryLetterCode|string |通信地址国家/地区字母代码 (两个字符的单词)|
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

