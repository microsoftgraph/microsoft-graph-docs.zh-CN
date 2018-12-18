---
title: userActivationCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: dkershaw10
ms.openlocfilehash: 396f6182d000df6d701e8c0cbad3dd02a258c4c0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322916"
---
# <a name="useractivationcounts-resource-type"></a>userActivationCounts 资源类型

## <a name="properties"></a>属性

| 属性          | 类型   | 说明                              |
| :---------------- | :----- | ---------------------------------------- |
| productType       | 字符串 | 产品类型，如"Office 365 ProPlus"、"Project 客户端"或"Visio Pro for Office 365"。 |
| lastActivatedDate | 日期   | 最新的激活日期。       |
| windows           | Int64  | Windows 上激活计数。 此数值包括 Windows 中的任何计算机上的每个激活。 |
| mac               | Int64  | Mac OS 上激活计数。          |
| windows10Mobile   | Int64  | 在激活依靠 Windows 10 移动。 |
| ios               | Int64  | 在 iOS 激活计数。             |
| android           | Int64  | 在 Android 设备上激活计数。  |
| activatedOnSharedComputer   | Boolean | 如果用户使用该产品之前的共享计算机上，则为 true。 |

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
