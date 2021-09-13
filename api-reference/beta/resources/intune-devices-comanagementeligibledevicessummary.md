---
title: comanagementEligibleDevicesSummary 资源类型
description: 尚未记录
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 90f4cb5f33b0ea1c260d6b6acaffac46d3e08434
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59111038"
---
# <a name="comanagementeligibledevicessummary-resource-type"></a>comanagementEligibleDevicesSummary 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|comanagedCount|Int32|已注册的设备Co-Managed|
|eligibleCount|Int32|完全有资格使用 Co-Management|
|eligibleButNotAzureAdJoinedCount|Int32|有资格加入Co-Management尚未加入 Azure Active Directory|
|needsOsUpdateCount|Int32|在操作系统更新后有资格使用Co-Management的设备计数|
|ineligibleCount|Int32|不符合设备要求的设备Co-Management|

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



