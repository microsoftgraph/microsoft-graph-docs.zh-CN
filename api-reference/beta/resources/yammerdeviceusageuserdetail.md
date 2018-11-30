---
title: yammerDeviceUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 8812b61d974815fd1cdf1bbe1549a21193e5a2f4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048765"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a>yammerDeviceUsageUserDetail 资源类型

## <a name="properties"></a>属性

| 属性          | 类型    |
| :---------------- | :------ |
| reportRefreshDate | 日期    |
| userPrincipalName | 字符串  |
| displayName       | 字符串  |
| userState         | 字符串  |
| stateChangeDate   | 日期    |
| lastActivityDate  | 日期    |
| usedWeb           | 布尔 |
| usedWindowsPhone  | 布尔 |
| usedAndroidPhone  | 布尔 |
| usediPhone        | 布尔 |
| usediPad          | 布尔 |
| usedOthers        | 布尔 |
| reportPeriod      | String  |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userState": "String", 
  "stateChangeDate": "Date", 
  "lastActivityDate": "Date", 
  "usedWeb": true, 
  "usedWindowsPhone": true, 
  "usedAndroidPhone": true, 
  "usediPhone": true, 
  "usediPad": true, 
  "usedOthers": true, 
  "reportPeriod": "String"
}
```
