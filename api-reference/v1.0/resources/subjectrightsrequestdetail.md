---
title: subjectRightsRequestDetail 资源类型
description: 表示主题权限请求的详细信息，包括找到的项目数、审阅的项目数等。
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 9e332d53acdeea4eed7b970263547dd066974210
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60457245"
---
# <a name="subjectrightsrequestdetail-resource-type"></a>subjectRightsRequestDetail 资源类型

命名空间：microsoft.graph

表示主题权限请求的详细信息，包括找到的项目数、审阅的项目数等。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|excludedItemCount|Int64|从请求中排除的项目计数。|
|insightCounts|[keyValuePair](../resources/keyvaluepair.md) 集合|每个见解的项目数。|
|itemCount|Int64|找到的项目数。|
|itemNeedReview|Int64|需要审阅的项目计数。|
|productItemCounts|[keyValuePair](../resources/keyvaluepair.md) 集合|每个产品（如产品、Exchange、SharePoint、OneDrive 和 Teams）的项Teams。|
|signedOffItemCount|Int64|管理员注销的项目计数。|
|totalItemSize|Int64|项目总大小（以字节为单位）。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.subjectRightsRequestDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.subjectRightsRequestDetail",
      "itemCount": "Int64",
      "totalItemSize": "Int64",
      "itemNeedReview": "Int64",
      "signedOffItemCount": "Int64",
      "excludedItemCount": "Int64",
      "productItemCounts": [],
      "insightCounts": []
}
```

