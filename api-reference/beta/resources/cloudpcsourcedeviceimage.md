---
title: cloudPcSourceDeviceImage 资源类型
description: '与 Azure 订阅关联的源映像。 '
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 3de1c3582ca792225b6aa7e6d36b5b33594249e2
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766472"
---
# <a name="cloudpcsourcedeviceimage-resource-type"></a>cloudPcSourceDeviceImage 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

与 Azure 订阅关联的源映像。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|源图像的 ID。|
|displayName|String|源显示名称的源图像。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcSourceDeviceImage"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcSourceDeviceImage",
  "id": "String (identifier)",
  "displayName": "String"
}
```
