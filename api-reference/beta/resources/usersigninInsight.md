---
title: userSignInInsight 资源类型
description: 在Azure AD评论中，userSignInInsight 资源表示根据用户上次登录日期和时间向审阅者提供的见解。
author: shubhamguptacal
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ca84ef57b6bb2431210ab3a6a91e80b7089d86bf
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62112549"
---
# <a name="usersignininsight-resource-type"></a>usersignininsight 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

表示根据用户上次登录日期和时间向审阅者提供的见解。

继承自 [governanceInsight](governanceinsight.md)。

## <a name="properties"></a>属性
| 属性    | 类型   | 说明 |
| :---------------| :---------- | :---------- |
| lastSignInDateTime | DateTimeOffset | 指示用户上次登录时间 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userSignInInsight",
  "baseType": "microsoft.graph.governanceInsight"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userSignInInsight",
  "lastSignInDateTime": "DateTimeOffset"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "usersignininsight resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
