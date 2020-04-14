---
title: detailsInfo 资源类型
description: 可以包含有关关联的标识或系统的任何信息的属性包。
localization_priority: Normal
author: khotz
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f62a773bb65f5d323ad6f906e53467366f7956d0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463051"
---
# <a name="detailsinfo-resource-type"></a>detailsInfo 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

可以包含有关关联的标识或系统的任何信息的属性包。 这可能包括有关要预配的属性或源/目标系统的详细信息。

## <a name="properties"></a>属性
**DetailsInfo**资源是一个 JSON 字符串，其中包含诸如**ApplicationId**、 **ObjectId**和**UPN**等其他属性。 属性集根据要设置的资源类型的不同而不同。 [列表 provisioningObjectSummary](../api/provisioningobjectsummary-list.md)显示了这种情况的示例。

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.detailsInfo",
  "openType": true,
 "optionalProperties": [
 
 ],
}-->
``` json
{
  "@odata.type": "microsoft.graph.detailsInfo"
}
```
