---
title: vppLicensingType 资源类型
description: 包含 iOS 批量采购程序 (Vpp) 许可类型的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 21d19579ef55b74280b7d2ddb3acb445aa18b864
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49199999"
---
# <a name="vpplicensingtype-resource-type"></a>vppLicensingType 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含 iOS 批量采购程序 (Vpp) 许可类型的属性。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|supportUserLicensing|布尔值|程序是否支持用户许可类型。|
|supportDeviceLicensing|布尔值|程序是否支持设备许可类型。|
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
  "supportUserLicensing": true,
  "supportDeviceLicensing": true,
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```




