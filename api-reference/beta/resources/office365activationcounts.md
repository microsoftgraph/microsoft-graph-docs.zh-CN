---
title: office365ActivationCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: d396ee84e4af6606cfde3e5fc17ef02c0a9594f1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966578"
---
# <a name="office365activationcounts-resource-type"></a>office365ActivationCounts 资源类型

## <a name="properties"></a>属性

| 属性          | 类型   | 说明                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | 日期   | 内容的最新日期。          |
| productType       | String | 产品类型, 如 "Office 365 专业增强版"、"Project Client" 或 "Visio Pro for Office 365"。 |
| 时间           | Int64  | Windows 上的激活计数。 此数字包括任何 Windows 计算机上的每次激活。 |
| mac               | Int64  | Mac OS 上的激活计数。          |
| android           | Int64  | Android 设备上的激活计数。  |
| ios               | Int64  | IOS 上的激活计数。             |
| windows10Mobile   | Int64  | Windows 10 移动版上的激活计数。 |

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
