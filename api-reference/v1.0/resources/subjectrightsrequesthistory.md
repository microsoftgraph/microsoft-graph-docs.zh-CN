---
title: subjectRightsRequestHistory 资源类型
description: 表示主题权限请求的历史记录。
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: d8a990990d5b3935ab54d9abb6a5e22453af6965
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60457644"
---
# <a name="subjectrightsrequesthistory-resource-type"></a>subjectRightsRequestHistory 资源类型

命名空间：microsoft.graph

表示主题权限请求的历史记录。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|changedBy|[identitySet](../resources/identityset.md)|更改了主题权限请求的用户的标识。|
|eventDateTime|DateTimeOffset|实体更改的数据和时间。|
|stage|subjectRightsRequestStage|实体更改的阶段。 可取值为：`contentRetrieval`、`contentReview`、`generateReport`、`contentDeletion`、`caseResolved`、`unknownFutureValue`。|
|stageStatus|subjectRightsRequestStageStatus|实体更改时阶段的状态。 可取值为：`notStarted`、`current`、`completed`、`failed`、`unknownFutureValue`。|
|type|String|历史记录的类型。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.subjectRightsRequestHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.subjectRightsRequestHistory",
    "type": "String",
    "stage": "String",
    "stageStatus": "String",
    "eventDateTime": "String (timeStamp)",
    "changedBy": {
        "user": {
            "id": "String",
            "displayName": "String"
        }
    }
}
```

