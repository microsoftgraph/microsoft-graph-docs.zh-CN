---
title: securityBaselineStateSummary 资源类型
description: 帐户的安全基线的安全基线合规性状态摘要。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 67af97c477bd559080ce8aa1b10f5418614f716d8aa439b590680b8416bebf59
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54193662"
---
# <a name="securitybaselinestatesummary-resource-type"></a>securityBaselineStateSummary 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

帐户的安全基线的安全基线合规性状态摘要。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 securityBaselineStateSummary](../api/intune-deviceintent-securitybaselinestatesummary-get.md)|[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|读取 [securityBaselineStateSummary 对象的属性和](../resources/intune-deviceintent-securitybaselinestatesummary.md) 关系。|
|[更新 securityBaselineStateSummary](../api/intune-deviceintent-securitybaselinestatesummary-update.md)|[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|更新 [securityBaselineStateSummary 对象](../resources/intune-deviceintent-securitybaselinestatesummary.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的唯一标识符。|
|secureCount|Int32|安全设备的数量|
|notSecureCount|Int32|非安全设备的数量|
|unknownCount|Int32|未知设备的数量|
|errorCount|Int32|错误设备的数量|
|conflictCount|Int32|冲突设备的数量|
|notApplicableCount|Int32|不适用设备的数量|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineStateSummary",
  "id": "String (identifier)",
  "secureCount": 1024,
  "notSecureCount": 1024,
  "unknownCount": 1024,
  "errorCount": 1024,
  "conflictCount": 1024,
  "notApplicableCount": 1024
}
```




