---
title: iosWebContentFilterSpecificWebsitesAccess 资源类型
description: 代表 iOS Web 内容筛选器设置类型，这将 URL 的书签安装到 iOS 内置浏览器。 示例方案是在课堂教师希望学生导航在浏览器书签其 iOS 的设备和不能访问其他网站上配置的网站。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 3b117aca95c43f36c216d6249221d689ae2da325
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942694"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a>iosWebContentFilterSpecificWebsitesAccess 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

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





