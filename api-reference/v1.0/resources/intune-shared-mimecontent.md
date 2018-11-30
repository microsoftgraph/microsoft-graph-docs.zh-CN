---
title: mimeContent 资源类型
description: 包含通用 MIME 内容的属性。
ms.openlocfilehash: 7f25a1c16b86a45886cd763c1a8a3aa6142c47e2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009232"
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



