---
title: windowsUpdateRolloutSettings 资源类型
description: 存储 Windows 更新推出设置的复杂类型，包括优惠开始日期时间、优惠结束日期时间和每组产品/服务之间的天数。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 76ca74fc580886463edada3bd63a056ca6d3aef4
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61339477"
---
# <a name="windowsupdaterolloutsettings-resource-type"></a>windowsUpdateRolloutSettings 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

存储 Windows 更新推出设置的复杂类型，包括优惠开始日期时间、优惠结束日期时间和每组产品/服务之间的天数。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|offerStartDateTimeInUTC|DateTimeOffset|功能更新的开始日期和时间设置、更新和显示功能更新配置文件，例如：2020-06-09T10：00：00Z。|
|offerEndDateTimeInUTC|DateTimeOffset|功能更新针对功能更新配置文件设置的、更新和显示的发布日期和时间结束，例如：2020-06-09T10：00：00Z。|
|offerIntervalInDays|Int32|要针对功能更新配置文件设置、更新和显示的每组产品/服务之间的 () 天数，例如：如果 OfferStartDateTimeInUTC 为 2020-06-09T10：00：00Z，且 OfferIntervalInDays 为 1， 接下来两组优惠将在 2020-06-10T10：00：00Z (下一天与指定时间) 和 2020-06-11T10：00：00Z (下一天在同一指定时间) 中第二天（介于 1 天之间）连续进行每组产品/服务。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateRolloutSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateRolloutSettings",
  "offerStartDateTimeInUTC": "String (timestamp)",
  "offerEndDateTimeInUTC": "String (timestamp)",
  "offerIntervalInDays": 1024
}
```




