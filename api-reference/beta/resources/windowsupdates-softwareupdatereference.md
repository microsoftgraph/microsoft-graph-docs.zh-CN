---
title: softwareUpdateReference 资源类型
description: 表示特定更新内容。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 9278900d85bc1ec6fc626200f0bf814dd3097b34
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61860423"
---
# <a name="softwareupdatereference-resource-type"></a>softwareUpdateReference 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示特定更新内容。

在部署中，相同的 **softwareUpdateReference** 可能会导致设备接收不同的更新修订，但内容被视为与部署中所有设备的上下文等效。

所有软件更新引用作为以下派生类型之一存在 [：featureUpdateReference](../resources/windowsupdates-featureupdatereference.md) 和 [expeditedQualityUpdateReference](../resources/windowsupdates-expeditedqualityupdatereference.md)。

继承自 [deployableContent](../resources/windowsupdates-deployablecontent.md)。 [windowsUpdateReference 的基类型](../resources/windowsupdates-windowsupdatereference.md)。

这是一个抽象类型。

## <a name="properties"></a>属性
无。

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.softwareUpdateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.softwareUpdateReference"
}
```

