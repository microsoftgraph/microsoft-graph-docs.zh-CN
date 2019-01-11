---
title: skypeForBusinessDeviceUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 95f2f6cf1f3f6c54c4b6b4b39a7118cd8a94b224
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858378"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a>skypeForBusinessDeviceUsageUserDetail 资源类型

## <a name="properties"></a>属性

| 属性          | 类型    |
| :---------------- | :------ |
| reportRefreshDate | 日期    |
| userPrincipalName | 字符串  |
| lastActivityDate  | 日期    |
| usedWindows       | 布尔 |
| usedWindowsPhone  | 布尔 |
| usedAndroidPhone  | 布尔 |
| usediPhone        | 布尔 |
| usediPad          | 布尔 |
| reportPeriod      | String  |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "usedWindows": true, 
  "usedWindowsPhone": true, 
  "usedAndroidPhone": true, 
  "usediPhone": true, 
  "usediPad": true, 
  "reportPeriod": "String"
}
```
