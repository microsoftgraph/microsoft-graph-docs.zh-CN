---
title: iosHomeScreenItem 资源类型
description: 表示 iOS 主屏幕上的项
author: tfitzmac
ms.openlocfilehash: 6a8d71e01ca8f2c284bcc3eddd7eb39b87c025d7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328187"
---
# <a name="ioshomescreenitem-resource-type"></a>iosHomeScreenItem 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

表示 iOS 主屏幕上的项
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|应用的名称|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenItem",
  "displayName": "String"
}
```





