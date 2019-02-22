---
title: encryptionReportPolicyDetails 资源类型
description: 加密报告的策略详细信息
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d9232acd2a155169385956b9d20b3011c963090a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177915"
---
# <a name="encryptionreportpolicydetails-resource-type"></a>encryptionReportPolicyDetails 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

加密报告的策略详细信息

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|policyId|字符串|加密报告的策略 Id|
|policyName|字符串|加密报告的策略名称|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.encryptionReportPolicyDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.encryptionReportPolicyDetails",
  "policyId": "String",
  "policyName": "String"
}
```




