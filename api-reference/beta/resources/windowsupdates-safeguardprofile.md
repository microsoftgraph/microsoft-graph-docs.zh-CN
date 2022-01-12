---
title: safeguardProfile 资源类型
description: 介绍 () 保护设备时所针对的问题。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 95ad3d053afa1fb27190407d359055c47afd4135
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861113"
---
# <a name="safeguardprofile-resource-type"></a>safeguardProfile 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

介绍 () 保护设备时所针对的问题。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|category|microsoft.graph.windowsUpdates.safeguardCategory|指定安全措施的类别。 可能的值是 `likelyIssues` `unknownFutureValue` ：、。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.safeguardProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.safeguardProfile",
  "category": "String"
}
```

