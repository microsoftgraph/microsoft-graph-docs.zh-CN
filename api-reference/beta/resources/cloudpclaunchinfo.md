---
title: cloudPcLaunchInfo 资源类型
description: 包含用于连接云电脑的信息。
author: andrewku0409
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 546bd11263c3bdb9ac4421eb8f9eb3580e6af255
ms.sourcegitcommit: 4ef29d4a2cfa1ccc4a3da649e683377b17b90108
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2022
ms.locfileid: "65126338"
---
# <a name="cloudpclaunchinfo-resource-type"></a>cloudPcLaunchInfo 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含用于连接 [cloudPC](../resources/cloudpc.md) 的信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|cloudPcId|String|云电脑的唯一标识符。|
|cloudPcLaunchUrl|String|云电脑的连接 URL。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcLaunchInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcLaunchInfo",
  "cloudPcId": "String",
  "cloudPcLaunchUrl": "String"
}
```

