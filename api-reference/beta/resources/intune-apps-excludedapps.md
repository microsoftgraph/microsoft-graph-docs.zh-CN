---
title: excludedApps 资源类型
description: 包含用于排除 Office365 应用程序的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1d3cd9a159597689a64070181640415a6ce2fc61
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395676"
---
# <a name="excludedapps-resource-type"></a>excludedApps 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于排除 Office365 应用程序的属性。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|访问|Boolean|值为 if 或不应排除 MS Office Access。|
|excel|Boolean|值为 if 或不应排除 MS Office Excel。|
|groove|Boolean|如果值或不应排除 MS Office OneDrive for Business 的 Groove。|
|infoPath|Boolean|值为 if 或不应排除 MS Office InfoPath。|
|lync|Boolean|如果值或不应排除 MS Office Skype for Business-Lync。|
|oneDrive|Boolean|值为 if 或不应排除 MS Office OneDrive。|
|oneNote|Boolean|值为 if 或不应排除 MS Office OneNote。|
|outlook|Boolean|值为 if 或不应排除 MS Office Outlook。|
|powerPoint|Boolean|值为 if 或不应排除 MS Office PowerPoint。|
|publisher|Boolean|值为 if 或不应排除 MS Office Publisher。|
|sharePointDesigner|Boolean|值为 if 或不应排除 MS Office SharePointDesigner。|
|visio|Boolean|值为 if 或不应排除 MS Office Visio。|
|word|Boolean|值为 if 或不应排除 MS Office Word。|

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
  "visio": true,
  "word": true
}
```




