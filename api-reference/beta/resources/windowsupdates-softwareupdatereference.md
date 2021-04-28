---
title: softwareUpdateReference 资源类型
description: 表示特定更新内容。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 66f7f895bd3d7556ad5e3d35066236663b474f41
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067973"
---
# <a name="softwareupdatereference-resource-type"></a>softwareUpdateReference 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示特定更新内容。

在部署中，相同的 **softwareUpdateReference** 可能会导致设备接收不同的更新修订，但内容被视为与部署中所有设备的上下文等效。

所有软件更新引用作为以下派生类型之一存在 [：featureUpdateReference](../resources/windowsupdates-featureupdatereference.md)。

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

