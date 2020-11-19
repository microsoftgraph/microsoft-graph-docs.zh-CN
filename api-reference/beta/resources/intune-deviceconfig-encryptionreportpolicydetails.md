---
title: encryptionReportPolicyDetails 资源类型
description: 加密报告的策略详细信息
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 874af3d0bf98cbfc5884a4f3387eb8d55323acaf
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49294576"
---
# <a name="encryptionreportpolicydetails-resource-type"></a>encryptionReportPolicyDetails 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

加密报告的策略详细信息

## <a name="properties"></a>属性
|属性|类型|Description|
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




