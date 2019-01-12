---
title: androidMinimumOperatingSystem 资源类型
description: 包含 Android 移动应用需要的最低操作系统的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 94f11678ab43e5f8785cb6cc0eddf073105b3ce8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975608"
---
# <a name="androidminimumoperatingsystem-resource-type"></a>androidMinimumOperatingSystem 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含 Android 移动应用需要的最低操作系统的属性。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|v4_0|布尔值|版本 4.0 或更高版本。|
|v4_0_3|布尔值|版本 4.0.3 或更高版本。|
|v4_1|布尔值|版本 4.1 或更高版本。|
|v4_2|布尔值|版本 4.2 或更高版本。|
|v4_3|布尔值|版本 4.3 或更高版本。|
|v4_4|布尔值|版本 4.4 或更高版本。|
|v5_0|布尔值|版本 5.0 或更高版本。|
|v5_1|布尔值|版本 5.1 或更高版本。|
|v6_0|Boolean|版本 6.0 或更高版本。|
|v7_0|Boolean|7.0 版或更高版本。|
|v7_1|Boolean|7.1 或更高版本。|
|v8_0|布尔值|版本 8.0 或更高版本。|
|v8_1|布尔值|8.1 或更高版本。|
|v9_0|布尔值|版本 9.0 或更高版本。|

## <a name="relationships"></a>Relationships
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidMinimumOperatingSystem",
  "v4_0": true,
  "v4_0_3": true,
  "v4_1": true,
  "v4_2": true,
  "v4_3": true,
  "v4_4": true,
  "v5_0": true,
  "v5_1": true,
  "v6_0": true,
  "v7_0": true,
  "v7_1": true,
  "v8_0": true,
  "v8_1": true,
  "v9_0": true
}
```





