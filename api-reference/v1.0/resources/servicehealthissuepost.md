---
title: serviceHealthIssuePost 资源类型
description: 表示服务运行状况问题的历史文章。
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: a53f09c6fc32de1c65e52e2554aa89b634f2b0e3
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266896"
---
# <a name="servicehealthissuepost-resource-type"></a>serviceHealthIssuePost 资源类型

命名空间：microsoft.graph

表示服务运行状况问题 [中的历史文章](../resources/servicehealthissue.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|文章的发布时间。|
|description|[itemBody](../resources/itembody.md)|服务问题帖子的内容。|
|postType|postType|服务问题历史文章的帖子类型。 可取值为：`regular`、`quick`、`strategic`、`unknownFutureValue`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.serviceHealthIssuePost"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceHealthIssuePost",
  "createdDateTime": "String (timestamp)",
  "postType": "String",
  "description": {
    "@odata.type": "microsoft.graph.itemBody"
  }
}
```

