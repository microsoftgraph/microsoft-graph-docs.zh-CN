---
title: ocrSettings 资源类型
description: 表示电子数据展示事例的 OCR 设置。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: d4b15f7bef89c37f4debedb58ed48734f86b1bef
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839175"
---
# <a name="ocrsettings-resource-type"></a>ocrSettings 资源类型

命名空间：microsoft.graph.security



表示电子数据展示用例的光学字符识别 (OCR) 设置。


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|isEnabled|Boolean|指示是否为案例启用 OCR。|
|maxImageSize|Int32|将在 KB) 中处理的最大图像大小。|
|timeout|持续时间|OCR 引擎的超时持续时间。 更长的超时可能会增加 OCR 的成功率，但可能会增加总处理时间。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.ocrSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ocrSettings",
  "isEnabled": "Boolean",
  "maxImageSize": "Integer",
  "timeout": "String (duration)"
}
```

