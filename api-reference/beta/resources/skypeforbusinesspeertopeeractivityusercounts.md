---
title: skypeForBusinessPeerToPeerActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: ad3b409f3abc4cc9e7476825f9dbf5b7c2120d92
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046475"
---
# <a name="skypeforbusinesspeertopeeractivityusercounts-resource-type"></a>skypeForBusinessPeerToPeerActivityUserCounts 资源类型

## <a name="properties"></a>属性

| 属性          | 类型   |
| :---------------- | :----- |
| im                | Int64  |
| audio             | Int64  |
| video             | Int64  |
| 的        | Int64  |
| 文件传输      | Int64  |
| reportRefreshDate | 日期   |
| reportDate        | 日期   |
| reportPeriod      | String |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityUserCounts"
} -->

```json
{
  "im": 1024, 
  "audio": 1024, 
  "video": 1024, 
  "appSharing": 1024, 
  "fileTransfer": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
