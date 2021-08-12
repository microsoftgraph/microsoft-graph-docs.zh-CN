---
title: serviceHealthIssuePost 资源类型
description: 表示服务运行状况问题的历史文章。
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: c005beb7b27956cad6f42c7251bb15be7024415c5096d8f012a88049534b6cad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54243014"
---
# <a name="servicehealthissuepost-resource-type"></a>serviceHealthIssuePost 资源类型

命名空间：microsoft.graph

表示服务运行状况问题 [中的历史文章](../resources/servicehealthissue.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|文章的发布时间。|
|说明|[itemBody](../resources/itembody.md)|服务问题帖子的内容。|
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

