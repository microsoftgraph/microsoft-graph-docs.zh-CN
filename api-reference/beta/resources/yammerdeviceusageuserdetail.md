---
title: yammerDeviceUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 4a3232f87775f4e08e5296c21282e80ee2f1ee88
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128485"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a>yammerDeviceUsageUserDetail 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性          | 类型    |
| :---------------- | :------ |
| reportRefreshDate | 日期    |
| userPrincipalName | String  |
| displayName       | String  |
| userState         | String  |
| stateChangeDate   | 日期    |
| lastActivityDate  | 日期    |
| usedWeb           | Boolean |
| usedWindowsPhone  | Boolean |
| usedAndroidPhone  | Boolean |
| usediPhone        | Boolean |
| usediPad          | Boolean |
| usedOthers        | Boolean |
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


