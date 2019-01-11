---
title: office365ActivationCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 30386b3833b8140d4c602e27cb3a78f3a68670dc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824988"
---
# <a name="office365activationcounts-resource-type"></a>office365ActivationCounts 资源类型

## <a name="properties"></a>属性

| 属性          | 类型   | Description                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | 日期   | 内容最晚日期。          |
| productType       | 字符串 | 产品类型，如"Office 365 ProPlus"、"Project 客户端"或"Visio Pro for Office 365"。 |
| windows           | Int64  | Windows 上激活计数。 此数值包括 Windows 中的任何计算机上的每个激活。 |
| mac               | Int64  | Mac OS 上激活计数。          |
| android           | Int64  | 在 Android 设备上激活计数。  |
| ios               | Int64  | 在 iOS 激活计数。             |
| windows10Mobile   | Int64  | 在激活依靠 Windows 10 移动。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "productType": "String", 
  "windows": 1024, 
  "mac": 1024, 
  "android": 1024, 
  "ios": 1024, 
  "windows10Mobile": 1024
}
```
