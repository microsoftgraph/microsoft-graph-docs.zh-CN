---
title: updateManagementEnrollment 资源类型
description: 表示通过特定更新类别的服务注册到管理中。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 992cfc8ebf53db3b1f3aad7c3c997d02344a503b
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861581"
---
# <a name="updatemanagementenrollment-resource-type"></a>updateManagementEnrollment 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示通过特定更新类别的服务注册到管理中。

继承自 [updatableAssetEnrollment](../resources/windowsupdates-updatableassetenrollment.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
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

