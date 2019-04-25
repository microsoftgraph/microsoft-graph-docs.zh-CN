---
title: iosMinimumOperatingSystem 资源类型
description: 包含 iOS 移动应用需要的最低操作系统的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3775a9bbc9eee6bfef5dd1bef8235bf6fc770603
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552210"
---
# <a name="iosminimumoperatingsystem-resource-type"></a>iosMinimumOperatingSystem 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含 iOS 移动应用需要的最低操作系统的属性。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|v8_0|布尔值|版本 8.0 或更高版本。|
|v9_0|布尔值|版本 9.0 或更高版本。|
|v10_0|布尔值|版本 10.0 或更高版本。|
|v11_0|布尔值|版本 11.0 或更高版本。|
|v12_0|布尔值|版本12.0 或更高版本。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMinimumOperatingSystem",
  "v8_0": true,
  "v9_0": true,
  "v10_0": true,
  "v11_0": true,
  "v12_0": true
}
```





