---
title: ocrSettings 资源类型
description: 电子数据展示案例的 OCR 设置
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 648e0ad63f558f211591d1c8aa976c2689dd271d
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080746"
---
# <a name="ocrsettings-resource-type"></a>ocrSettings 资源类型

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

OCR (光学字符识别) 电子数据展示案例的设置。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|isEnabled|Boolean|指示是否对案例启用 OCR。|
|maxImageSize|Int32|将处理的最大图像大小（以 KB 为单位) 。|
|timeout|期限|OCR 引擎的超时持续时间。 较长的超时可能会增加 OCR 的成功，但会增加总处理时间。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.ediscovery.ocrSettings"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.ocrSettings",
  "isEnabled": "Boolean",
  "maxImageSize": "Integer",
  "timeout": "String (duration)"
}
```
