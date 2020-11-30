---
title: cloudPcSourceDeviceImage 资源类型
description: '与你的 Azure 订阅关联的源映像。 '
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: eddae0ed023fb60c290067f3520ef90a67dec23b
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378277"
---
# <a name="cloudpcsourcedeviceimage-resource-type"></a>cloudPcSourceDeviceImage 资源类型

命名空间：microsoft.graph

与你的 Azure 订阅关联的源映像。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|源图像的 ID。|
|displayName|字符串|源图像的显示名称。|

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
