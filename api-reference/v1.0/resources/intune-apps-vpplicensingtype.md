---
title: vppLicensingType 资源类型
description: 包含 iOS 批量采购程序 (Vpp) 许可类型的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 34314ee04dacbc422b2a9b09e8f6802d308c3d69
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971471"
---
# <a name="vpplicensingtype-resource-type"></a>vppLicensingType 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含 iOS 批量采购程序 (Vpp) 许可类型的属性。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|supportsUserLicensing|布尔值|程序是否支持用户许可类型。|
|supportsDeviceLicensing|布尔值|程序是否支持设备许可类型。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppLicensingType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```



