---
title: updateManagementEnrollment 资源类型
description: 表示通过特定更新类别的服务注册到管理中。
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 8d780894e90a1f6eec748a9f62f486b39d3c6cfb
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890183"
---
# <a name="updatemanagementenrollment-resource-type"></a>updateManagementEnrollment 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示通过特定更新类别的服务注册到管理中。

继承自 [updatableAssetEnrollment](../resources/windowsupdates-updatableassetenrollment.md)。

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|updateCategory|microsoft.graph.windowsUpdates.updateCategory|服务管理的更新类别。 支持 **updateCategory** 值的子集。 可取值为：`feature`、`unknownFutureValue`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.updateManagementEnrollment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.updateManagementEnrollment",
  "updateCategory": "String"
}
```

