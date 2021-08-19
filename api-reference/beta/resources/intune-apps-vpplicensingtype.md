---
title: vppLicensingType 资源类型
description: 包含 iOS 批量采购程序 (Vpp) 许可类型的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6eca0f098d29d217e378ada2dcc85535eb39283b67b43fb1ac184f4b73fb9ff3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54227622"
---
# <a name="vpplicensingtype-resource-type"></a>vppLicensingType 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

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




