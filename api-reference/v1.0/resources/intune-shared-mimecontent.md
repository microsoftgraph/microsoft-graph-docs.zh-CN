---
title: mimeContent 资源类型
description: 包含通用 MIME 内容的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8a486753c95afce9dff6ceec5846ff618b9103b3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971898"
---
# <a name="mimecontent-resource-type"></a>mimeContent 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含通用 MIME 内容的属性。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|type|String|指示内容 MIME 类型。|
|值|Binary|包含实际内容的字节数组。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mimeContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mimeContent",
  "type": "String",
  "value": "binary"
}
```



