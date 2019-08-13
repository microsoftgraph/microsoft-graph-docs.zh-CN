---
title: excludedApps 资源类型
description: 包含已排除的 Office365 应用程序的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d566cd8ba088568e27c9a7e4878eda54cd7f1252
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366089"
---
# <a name="excludedapps-resource-type"></a>excludedApps 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含已排除的 Office365 应用程序的属性。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|访问|Boolean|如果应排除 MS Office Access, 则该值为。|
|excel|Boolean|如果不应排除 MS Office Excel 的值, 则为。|
|为止|Boolean|如果要排除 MS Office OneDrive for Business-Groove 的值, 应将其排除。|
|infoPath|Boolean|如果不应排除 MS Office InfoPath, 则值为。|
|lync|Boolean|如果要排除 MS Office Skype for Business-Lync 的值, 应将其排除。|
|For|Boolean|如果不应排除 MS Office OneDrive, 则值为。|
|oneNote|Boolean|如果不应排除 MS Office OneNote 的值, 则为。|
|outlook|Boolean|如果不应排除 MS Office Outlook 的值, 则为。|
|powerPoint|Boolean|如果不应排除 MS Office PowerPoint, 则值为。|
|发布者|Boolean|应排除 MS Office 发布服务器的值。|
|sharePointDesigner|Boolean|如果不应排除 MS Office SharePointDesigner 的值, 则为。|
|协作|Boolean|如果不应排除 MS Office 团队, 则值为。|
|visio|Boolean|应排除 MS Office Visio 的值。|
|word|Boolean|如果不应排除 MS Office Word 的值, 则为。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.excludedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.excludedApps",
  "access": true,
  "excel": true,
  "groove": true,
  "infoPath": true,
  "lync": true,
  "oneDrive": true,
  "oneNote": true,
  "outlook": true,
  "powerPoint": true,
  "publisher": true,
  "sharePointDesigner": true,
  "teams": true,
  "visio": true,
  "word": true
}
```



