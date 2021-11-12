---
title: printUsageByUser 资源类型
description: 描述指定时间段内用户的打印活动 (usageDate) 。
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: f702c0dcb81d1b88f2c9bb0e314e74b97a905004
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60936101"
---
# <a name="printusagebyuser-resource-type"></a>printUsageByUser 资源类型

命名空间：microsoft.graph

描述指定时间段内用户的打印活动 (usageDate) 。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
| [列出 (每天) ](../api/reportroot-list-dailyprintusagebyuser.md) | [printUsageByUser](printusagebyuser.md) | 获取每日打印使用情况摘要的列表，按用户分组。 |
| [列出 (月) ](../api/reportroot-list-monthlyprintusagebyuser.md) | [printUsageByUser](printusagebyuser.md) | 获取按用户分组的每月打印使用情况摘要列表。 |
| [获取](../api/printusagebyuser-get.md) | [printUsageByUser](printusagebyuser.md) | 读取 printUsageByUser 对象的属性和关系。 |

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|此使用率摘要的 ID。|
|userPrincipalName|String|这些统计信息所代表的用户的 UPN。|
|usageDate|日期|与这些统计信息关联的日期。|
|completedBlackAndWhiteJobCount|Int64|在关联的日期代表用户完成的黑白打印作业数。|
|completedColorJobCount|Int64|在关联的日期代表用户完成的颜色打印作业数。|
|incompleteJobCount|Int64|代表用户（但不在关联日期）排队的打印作业数。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printUsageByUser",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printUsageByUser",
  "id": "String (identifier)",
  "usageDate": "Date",
  "completedBlackAndWhiteJobCount": "Integer",
  "completedColorJobCount": "Integer",
  "incompleteJobCount": "Integer",
  "userPrincipalName": "String"
}
```

