---
title: excludedApps 资源类型
description: 包含用于排除 Office365 应用程序的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 90216c639d36a989b2fad5dbdc1adbd11fe46ede
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943947"
---
# <a name="excludedapps-resource-type"></a>excludedApps 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

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

## <a name="relationships"></a>Relationships
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





