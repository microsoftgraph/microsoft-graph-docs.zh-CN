---
title: vppLicensingType 资源类型
description: 包含 iOS 批量采购程序 (Vpp) 许可类型的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 812cbdc203b09422f8a2cddac205d59f8c762a34
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949708"
---
# <a name="vpplicensingtype-resource-type"></a>vppLicensingType 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

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




