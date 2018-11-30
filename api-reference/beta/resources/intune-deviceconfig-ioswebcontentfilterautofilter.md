---
title: iosWebContentFilterAutoFilter 资源类型
description: 代表 iOS Web 内容筛选器设置类型，它使 iOS 自动筛选功能并允许其他 URL 访问控制。 没有属性值来构造，iOS 设备将启用自动筛选器无论。
ms.openlocfilehash: 04a221ac512ab3934702a2a9e3178ba23a2ac3ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047078"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a>iosWebContentFilterAutoFilter 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

代表 iOS Web 内容筛选器设置类型，它使 iOS 自动筛选功能并允许其他 URL 访问控制。 没有属性值来构造，iOS 设备将启用自动筛选器无论。

继承自[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|allowedUrls|String 集合|允许的访问的其他 Url|
|blockedUrls|String 集合|阻止访问的其他 Url|

## <a name="relationships"></a>Relationships
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosWebContentFilterAutoFilter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWebContentFilterAutoFilter",
  "allowedUrls": [
    "String"
  ],
  "blockedUrls": [
    "String"
  ]
}
```





