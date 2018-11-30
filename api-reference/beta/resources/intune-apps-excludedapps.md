---
title: excludedApps 资源类型
description: 包含用于排除 Office365 应用程序的属性。
ms.openlocfilehash: 05c1ed7f4789e1a27ddacf92dbd773b2f5a21847
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043898"
---
# <a name="excludedapps-resource-type"></a>excludedApps 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含用于排除 Office365 应用程序的属性。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|访问|布尔|值为 if 或不应排除 MS Office Access。|
|excel|布尔|值为 if 或不应排除 MS Office Excel。|
|groove|布尔|如果值或不应排除 MS Office OneDrive for Business 的 Groove。|
|infoPath|布尔|值为 if 或不应排除 MS Office InfoPath。|
|lync|布尔|如果值或不应排除 MS Office Skype for Business-Lync。|
|oneDrive|布尔|值为 if 或不应排除 MS Office OneDrive。|
|oneNote|布尔|值为 if 或不应排除 MS Office OneNote。|
|outlook|布尔|值为 if 或不应排除 MS Office Outlook。|
|powerPoint|布尔|值为 if 或不应排除 MS Office PowerPoint。|
|publisher|布尔|值为 if 或不应排除 MS Office Publisher。|
|sharePointDesigner|布尔|值为 if 或不应排除 MS Office SharePointDesigner。|
|visio|布尔|值为 if 或不应排除 MS Office Visio。|
|word|布尔|值为 if 或不应排除 MS Office Word。|

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





