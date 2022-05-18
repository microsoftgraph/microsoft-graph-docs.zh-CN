---
title: subjectRightsRequestEnumeratedSiteLocation 资源类型
description: 表示主题权限请求的属性，该请求定义特定网站 (SharePoint网站、OneDrive for Business网站和Microsoft Teams通道) 作为搜索位置。
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: b7b8752fb51da3eaaa9762de7b38cf080559a5e4
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461681"
---
# <a name="subjectrightsrequestenumeratedsitelocation-resource-type"></a>subjectRightsRequestEnumeratedSiteLocation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示主题权限请求的属性，该请求定义特定网站 (SharePoint网站、OneDrive for Business网站和Microsoft Teams通道) 作为搜索位置。

继承自 [subjectRightsRequestSiteLocation](../resources/subjectrightsrequestsitelocation.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|urls|String collection|应包含的网站 URL 的集合。 包括每个站点的 URL，例如 `https://www.contoso.com/site1`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.subjectRightsRequestEnumeratedSiteLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.subjectRightsRequestEnumeratedSiteLocation",
  "urls": [
    "String"
  ]
}
```

