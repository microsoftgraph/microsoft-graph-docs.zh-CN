---
title: detailsInfo 资源类型
description: 可以包含有关关联标识或系统的任何信息的属性包。
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: e5beb5d281186b16acfa38087b6ee2d9ed3f0058f972aaeba2941467c545f523
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54130378"
---
# <a name="detailsinfo-resource-type"></a>detailsInfo 资源类型

命名空间：microsoft.graph

可以包含有关关联标识或系统的任何信息的属性包。 这可能包括有关正在设置的属性或源/目标系统的详细信息。

## <a name="properties"></a>属性
**detailsInfo** 资源是一个 JSON 字符串，其中包含其他属性，如 **ApplicationId、ObjectId** 和 **UPN**。 属性集因所设置的资源类型而异。 [List provisioningObjectSummary](../api/provisioningobjectsummary-list.md) 显示了这一点的示例。

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


