---
title: office365ActivationCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 39e679da134120377f17dab520c332dc54aab328ef924b65212f5145279a8402
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54176321"
---
# <a name="office365activationcounts-resource-type"></a>office365ActivationCounts 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性          | 类型   | 说明                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | 日期   | 内容的最新日期。          |
| productType       | String | 产品类型，例如"Microsoft 365 ProPlus"或"Project Client"。 |
| windows           | Int64  | 激活次数Windows。 此数字包括任何计算机Windows激活。 |
| mac               | Int64  | Mac 操作系统上的激活计数。          |
| android           | Int64  | Android 设备上的激活计数。  |
| ios               | Int64  | iOS 上的激活计数。             |
| windows10Mobile   | Int64  | 移动版上的Windows 10计数。 |

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


