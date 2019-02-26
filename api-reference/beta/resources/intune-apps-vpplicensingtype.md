---
title: vppLicensingType 资源类型
description: 包含 iOS 批量采购程序 (Vpp) 许可类型的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f09ca9a8f891b90563ebad2cff74775f4c6fb7c2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168395"
---
# <a name="vpplicensingtype-resource-type"></a>vppLicensingType 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含 iOS 批量采购程序 (Vpp) 许可类型的属性。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|supportUserLicensing|Boolean|程序是否支持用户许可类型。|
|supportDeviceLicensing|布尔值|程序是否支持设备许可类型。|
|supportsUserLicensing|Boolean|程序是否支持用户许可类型。|
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
  "supportUserLicensing": true,
  "supportDeviceLicensing": true,
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```




