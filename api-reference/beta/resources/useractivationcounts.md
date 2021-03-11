---
title: userActivationCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: jpettere
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 719a73739a64dca2bd7a052cc9cdd51007173eff
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719897"
---
# <a name="useractivationcounts-resource-type"></a>userActivationCounts 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性          | 类型   | 说明                              |
| :---------------- | :----- | ---------------------------------------- |
| productType       | String | 产品类型，例如"Microsoft 365 ProPlus"或"Project Client"。 |
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


