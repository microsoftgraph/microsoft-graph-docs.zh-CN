---
title: iosWebContentFilterAutoFilter 资源类型
description: 表示 ios Web 内容筛选器设置类型, 该类型启用 ios 自动筛选功能并允许其他 URL 访问控制。 在不使用属性值的情况下构建时, iOS 设备将启用自动筛选器 (而不考虑)。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 91efedb47fff71a66d12e0d2c976d61fab2fa76c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460413"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a>iosWebContentFilterAutoFilter 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 ios Web 内容筛选器设置类型, 该类型启用 ios 自动筛选功能并允许其他 URL 访问控制。 在不使用属性值的情况下构建时, iOS 设备将启用自动筛选器 (而不考虑)。


继承自[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|allowedUrls|String collection|允许访问的其他 url|
|blockedUrls|String collection|为 access 阻止的其他 url|

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





