---
title: cloudPcSourceDeviceImage 资源类型
description: '与你的 Azure 订阅关联的源映像。 '
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: c944ab1a634d10e978c6ce1620ebe1accc5e4359
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563742"
---
# <a name="cloudpcsourcedeviceimage-resource-type"></a>cloudPcSourceDeviceImage 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

与你的 Azure 订阅关联的源映像。

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|源图像的 ID。|
|displayName|String|源图像的显示名称。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcSourceDeviceImage",
  "baseType": "microsoft.graph.entity"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcSourceDeviceImage",
  "id": "String (identifier)",
  "displayName": "String"
}
```
