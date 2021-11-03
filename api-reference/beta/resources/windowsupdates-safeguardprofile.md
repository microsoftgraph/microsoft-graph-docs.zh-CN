---
title: safeguardProfile 资源类型
description: 介绍 () 保护设备时所针对的问题。
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: d6df910ceff9e726c9a6aae3b847aa0478a7b107
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60697168"
---
# <a name="safeguardprofile-resource-type"></a>safeguardProfile 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

介绍 () 保护设备时所针对的问题。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|category|microsoft.graph.windowsUpdates.safeguardCategory|指定安全措施的类别。 可能的值是 `likelyIssues` ：。|

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

