---
title: siteSettings 资源类型
description: 表示网站的设置。
author: k-tsoi
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 210b0f36d0dbbfc9402eec6d0a58a62ae646605a
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589763"
---
# <a name="sitesettings-resource-type"></a>siteSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示网站的 [设置]。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|languageTag|String|此网站上使用的语言的语言标记。|
|timeZone|String|指示网站时区从协调世界时与 UTC 时间 (的时间) 。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.siteSettings"
}
-->
``` json
{
    "languageTag": "String",
    "timeZone": "String"
}
```

[网站]: site.md
