---
title: excludedApps 资源类型
description: 包含已排除的 Office365 应用程序的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 89a6504781f64cf0838474ec587e2495c875062c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730782"
---
# <a name="excludedapps-resource-type"></a>excludedApps 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含已排除的 Office365 应用程序的属性。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|访问|布尔|如果应排除 MS Office Access，则该值为。|
|必应|布尔|如果应排除 Microsoft 搜索为默认值，则为。|
|excel|布尔|如果不应排除 MS Office Excel 的值，则为。|
|为止|布尔|如果要排除 MS Office OneDrive for Business-Groove 的值，应将其排除。|
|infoPath|布尔|如果不应排除 MS Office InfoPath，则值为。|
|lync|布尔|如果要排除 MS Office Skype for Business-Lync 的值，应将其排除。|
|For|布尔|如果不应排除 MS Office OneDrive，则值为。|
|oneNote|布尔|如果不应排除 MS Office OneNote 的值，则为。|
|outlook|布尔|如果不应排除 MS Office Outlook 的值，则为。|
|powerPoint|布尔|如果不应排除 MS Office PowerPoint，则值为。|
|发布者|布尔|应排除 MS Office 发布服务器的值。|
|sharePointDesigner|布尔|如果不应排除 MS Office SharePointDesigner 的值，则为。|
|协作|布尔|如果不应排除 MS Office 团队，则值为。|
|visio|布尔|应排除 MS Office Visio 的值。|
|word|布尔|如果不应排除 MS Office Word 的值，则为。|

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
  "bing": true,
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





