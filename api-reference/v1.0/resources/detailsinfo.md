---
title: detailsInfo 资源类型
description: 可以包含有关关联标识或系统的任何信息的属性包。
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 1841c513651131c4bf624c07ee117fae32df79f7
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240763"
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


