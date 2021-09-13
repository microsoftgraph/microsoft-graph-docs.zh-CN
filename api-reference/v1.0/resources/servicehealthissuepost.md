---
title: serviceHealthIssuePost 资源类型
description: 表示服务运行状况问题的历史文章。
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 3216f0a4510b6dd66a0ce5c7a96834dbf289b378
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59126672"
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

