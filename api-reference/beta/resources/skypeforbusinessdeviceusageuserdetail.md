---
title: skypeForBusinessDeviceUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 50f37fdfd3441c256241b76ebcc6b144eb1486d7
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811047"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a>skypeForBusinessDeviceUsageUserDetail 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性          | 类型    |
| :---------------- | :------ |
| reportRefreshDate | 日期    |
| userPrincipalName | String  |
| lastActivityDate  | 日期    |
| usedWindows       | 布尔值 |
| usedWindowsPhone  | 布尔值 |
| usedAndroidPhone  | 布尔值 |
| usediPhone        | 布尔值 |
| usediPad          | 布尔值 |
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
