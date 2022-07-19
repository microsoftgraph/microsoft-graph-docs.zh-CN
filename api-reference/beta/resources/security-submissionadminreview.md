---
title: submissionAdminReview 资源类型
description: 表示威胁提交管理员评审信息
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 410ffc88cb5d5fade44456b928996834c7722cac
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856636"
---
# <a name="submissionadminreview-resource-type"></a>submissionAdminReview 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示威胁提交管理员审阅信息。 目前，仅支持用户报告的电子邮件威胁提交，管理员可以对其进行评审。

## <a name="properties"></a>属性
| 属性       | 类型                     | Description                                  |
|:---------------|:-------------------------|:---------------------------------------------|
| reviewBy       | String                   | 指定查看电子邮件的人员。 标识是电子邮件 ID 或其他标识字符串。|
| reviewDateTime | DateTimeOffset           | 指定审查发生的日期时间。|
| reviewResult   | submissionResultCategory | 指定评审结果。 可能的值是：`notJunk`、、`spam`、`phishing`、`allowedByPolicy``malware`、`blockedByPolicy`、`spoof``unknown`、`noResultAvailable`和 `unknownFutureValue`。  |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.submissionAdminReview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.submissionAdminReview",
  "reviewDateTime": "String (timestamp)",
  "reviewResult": "String",
  "reviewBy": "String"
}
```

