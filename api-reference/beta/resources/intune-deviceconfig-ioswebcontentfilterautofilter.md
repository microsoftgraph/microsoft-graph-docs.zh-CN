---
title: iosWebContentFilterAutoFilter 资源类型
description: 表示 iOS Web 内容筛选器设置类型，启用 iOS 自动筛选功能并允许进行其他 URL 访问控制。 当构建时没有属性值，iOS 设备将启用自动筛选器，而不管如何。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4c88850a9cb9cfab27da02231a908ed9466b6389
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59127232"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a>iosWebContentFilterAutoFilter 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 iOS Web 内容筛选器设置类型，启用 iOS 自动筛选功能并允许进行其他 URL 访问控制。 当构建时没有属性值，iOS 设备将启用自动筛选器，而不管如何。


继承自 [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|allowedUrls|字符串集合|允许访问的其他 URL|
|blockedUrls|字符串集合|阻止访问的其他 URL|

## <a name="relationships"></a>关系
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



