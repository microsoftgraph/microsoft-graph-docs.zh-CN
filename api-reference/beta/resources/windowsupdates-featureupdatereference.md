---
title: featureUpdateReference 资源类型
description: 表示Windows 10更新内容。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 21fcec33dd0072aed12205f44a24eac7c4ba7569
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61836662"
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

