---
title: updateManagementEnrollment 资源类型
description: 表示通过特定更新类别的服务注册到管理中。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 1d00bc152d5fc3b7b4be267cd3ea56fab52b8b38
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067298"
---
# <a name="updatemanagementenrollment-resource-type"></a>updateManagementEnrollment 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示通过特定更新类别的服务注册到管理中。

继承自 [updatableAssetEnrollment](../resources/windowsupdates-updatableassetenrollment.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|updateCategory|microsoft.graph.windowsUpdates.updateCategory|服务管理的更新类别。 支持 **updateCategory** 值的子集。 可能的值是 `feature` ：。|

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

