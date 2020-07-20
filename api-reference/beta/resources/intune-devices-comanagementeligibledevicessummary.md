---
title: comanagementEligibleDevicesSummary 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 55df0591dfcbabd997dfda1bb07dbd116c14dcbe
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793449"
---
# <a name="comanagementeligibledevicessummary-resource-type"></a>comanagementEligibleDevicesSummary 资源类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|comanagedCount|Int32|已进行共同管理的设备的计数|
|eligibleCount|Int32|完全符合共同管理条件的设备的数量|
|eligibleButNotAzureAdJoinedCount|Int32|符合共同管理但尚未加入 Azure Active Directory 的设备的计数|
|needsOsUpdateCount|Int32|在 OS 更新之后符合共同管理条件的设备的计数|
|ineligibleCount|Int32|不符合共同管理要求的设备的计数|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.comanagementEligibleDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.comanagementEligibleDevicesSummary",
  "comanagedCount": 1024,
  "eligibleCount": 1024,
  "eligibleButNotAzureAdJoinedCount": 1024,
  "needsOsUpdateCount": 1024,
  "ineligibleCount": 1024
}
```



