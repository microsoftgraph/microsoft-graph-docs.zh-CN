---
title: detailsInfo 资源类型
description: 可以包含有关关联的标识或系统的任何信息的属性包。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9d3a6726c2151376d858f7962527e4dc6f9b53e7
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349340"
---
# <a name="detailsinfo-resource-type"></a>detailsInfo 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

可以包含有关关联的标识或系统的任何信息的属性包。 这可能包括有关要预配的属性或源/目标系统的详细信息。

## <a name="properties"></a>属性
**DetailsInfo**资源是一个 JSON 字符串, 其中包含诸如**ApplicationId**、 **ObjectId**和**UPN**等其他属性。 属性集根据要设置的资源类型的不同而不同。 [列表 provisioningObjectSummary](../api/provisioningobjectsummary-list.md)显示了这种情况的示例。

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
