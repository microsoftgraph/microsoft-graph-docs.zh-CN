---
title: macOSMinimumOperatingSystem 资源类型
description: 最低操作系统要求 MacOS 应用程序。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 05ea05d85ac12db5be6fc5eb18eff3bca0c87556
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938088"
---
# <a name="macosminimumoperatingsystem-resource-type"></a>macOSMinimumOperatingSystem 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

最低操作系统要求 MacOS 应用程序。
## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|v10_7|布尔|Mac OS 10.7 或更高版本。|
|v10_8|布尔|Mac OS 10.8 或更高版本。|
|v10_9|布尔|Mac OS 10.9 或更高版本。|
|v10_10|布尔|Mac OS 10.10 或更高版本。|
|v10_11|布尔|Mac OS 10.11 或更高版本。|
|v10_12|布尔|Mac OS 10.12 或更高版本。|
|v10_13|布尔|Mac OS 10.13 或更高版本。|

## <a name="relationships"></a>Relationships
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSMinimumOperatingSystem",
  "v10_7": true,
  "v10_8": true,
  "v10_9": true,
  "v10_10": true,
  "v10_11": true,
  "v10_12": true,
  "v10_13": true
}
```





