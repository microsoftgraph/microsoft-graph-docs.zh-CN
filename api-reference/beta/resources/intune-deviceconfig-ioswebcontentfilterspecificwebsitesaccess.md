---
title: iosWebContentFilterSpecificWebsitesAccess 资源类型
description: 代表 iOS Web 内容筛选器设置类型，这将 URL 的书签安装到 iOS 内置浏览器。 示例方案是在课堂教师希望学生导航在浏览器书签其 iOS 的设备和不能访问其他网站上配置的网站。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 964ade2d2b46755fbba2903c6e9607340f60aedf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424761"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a>iosWebContentFilterSpecificWebsitesAccess 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

代表 iOS Web 内容筛选器设置类型，这将 URL 的书签安装到 iOS 内置浏览器。 示例方案是在课堂教师希望学生导航在浏览器书签其 iOS 的设备和不能访问其他网站上配置的网站。


继承自[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|specificWebsitesOnly|[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)集合|将内置的浏览器和用户安装 URL 书签只允许通过书签访问网站。 该集合最多可包含 500 个元素。|
|websiteList|[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)集合|将内置的浏览器和用户安装 URL 书签只允许通过书签访问网站。 该集合最多可包含 500 个元素。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosWebContentFilterSpecificWebsitesAccess"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWebContentFilterSpecificWebsitesAccess",
  "specificWebsitesOnly": [
    {
      "@odata.type": "microsoft.graph.iosBookmark",
      "url": "String",
      "bookmarkFolder": "String",
      "displayName": "String"
    }
  ],
  "websiteList": [
    {
      "@odata.type": "microsoft.graph.iosBookmark",
      "url": "String",
      "bookmarkFolder": "String",
      "displayName": "String"
    }
  ]
}
```




