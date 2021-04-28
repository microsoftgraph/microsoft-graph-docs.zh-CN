---
title: featureUpdateReference 资源类型
description: 表示Windows 10更新内容。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 69eda05a94982429035999bd914c6f0c9847fa67
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067331"
---
# <a name="featureupdatereference-resource-type"></a>featureUpdateReference 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示Windows 10更新内容。

在部署中，相同的功能更新引用可能会导致设备接收不同的更新修订，但内容被视为与部署中所有设备的上下文等效。

继承自 [windowsUpdateReference](../resources/windowsupdates-windowsupdatereference.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|version|String|按版本指定功能更新。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.featureUpdateReference",
  "version": "String"
}
```

