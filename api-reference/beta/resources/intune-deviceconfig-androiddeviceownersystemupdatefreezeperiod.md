---
title: androidDeviceOwnerSystemUpdateFreezePeriod 资源类型
description: 表示 Android 设备所有者系统更新冻结时段列表中的一项
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 54c3d150a579f981eccbe03dfccddfaf8b02b701
ms.sourcegitcommit: 00ac72f7b1cdde4f71ff332c2e7953908ef9de52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/04/2022
ms.locfileid: "61712170"
---
# <a name="androiddeviceownersystemupdatefreezeperiod-resource-type"></a>androidDeviceOwnerSystemUpdateFreezePeriod 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 Android 设备所有者系统更新冻结时段列表中的一项

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|startMonth|Int32|冻结期开始日期的月份。 有效值为 1 到 12|
|startDay|Int32|冻结期开始日期的日期。 有效值为 1 到 31|
|endMonth|Int32|冻结期结束日期的月份。 有效值为 1 到 12|
|endDay|Int32|冻结期结束日期的日期。 有效值为 1 到 31|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerSystemUpdateFreezePeriod"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerSystemUpdateFreezePeriod",
  "startMonth": 1024,
  "startDay": 1024,
  "endMonth": 1024,
  "endDay": 1024
}
```




