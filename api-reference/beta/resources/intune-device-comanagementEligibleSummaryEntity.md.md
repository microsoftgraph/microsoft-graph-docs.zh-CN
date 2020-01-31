---
title: comanagementEligibleSummaryEntity 资源类型
description: comanagementEligibleSummaryEntity 资源类型
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 80c2afff56d845097990ef927a743678a248c9fd
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636579"
---
# <a name="comanagementeligiblesummaryentity-resource-type"></a>comanagementEligibleSummaryEntity 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

给定设备的托管设备移动应用配置状态。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 comanagementEligibleSummaryEntity](../api/intune-device-comanagementEligibleSummaryEntity-list.md)|comanagementEligibleSummaryEntity 集合|列出 comanagementEligibleSummaryEntity 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|EligibleDeviceSummaryEntity 的唯一 Id|
|coManagedCount|Int32|已 CoManaged 的设备计数|
|eligibleCount|Int32|完全符合条件的设备计数 CoManagement|
|eligibleButNotAadJoinedCount|Int32|符合 CoManagement 但尚未加入 Azure Active Directory 的设备的计数|
|needsOSUpdateCount|Int32|在 OS 更新后符合 CoManagement 条件的设备的计数|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.comanagementEligibleSummaryEntity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.comanagementEligibleSummaryEntity",
  "id": "String (identifier)",
  "coManagedCount": 1024,
  "eligibleCount": 1024,
  "eligibleButNotAadJoinedCount": 1024,
  "needsOSUpdateCount": 1024
}
```

