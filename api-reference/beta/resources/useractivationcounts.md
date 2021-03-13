---
title: userActivationCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 48adb73bac65ddced88aea3edb18deae7653f5b3
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761791"
---
# <a name="useractivationcounts-resource-type"></a>userActivationCounts 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性          | 类型   | 说明                              |
| :---------------- | :----- | ---------------------------------------- |
| productType       | String | 产品类型，例如"Microsoft 365 专业增强版"或"Project 客户端"。 |
| lastActivatedDate | 日期   | 最新激活的日期。       |
| windows           | Int64  | Windows 上的激活计数。 此数字包括任何 Windows 计算机上每次激活。 |
| mac               | Int64  | Mac 操作系统上的激活计数。          |
| windows10Mobile   | Int64  | Windows 10 移动版上的激活计数。 |
| ios               | Int64  | iOS 上的激活计数。             |
| android           | Int64  | Android 设备上的激活计数。  |
| activatedOnSharedComputer   | 布尔 | 如果用户之前在共享计算机上使用过该产品，则其为 True。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userActivationCounts"
} -->

```json
{
  "productType": "String", 
  "lastActivatedDate": "Date", 
  "windows": 1024, 
  "mac": 1024, 
  "windows10Mobile": 1024, 
  "ios": 1024, 
  "android": 1024,
  "activatedOnSharedComputer": true 
}
```


