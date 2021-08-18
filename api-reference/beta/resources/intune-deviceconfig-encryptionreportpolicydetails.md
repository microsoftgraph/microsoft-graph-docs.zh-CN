---
title: encryptionReportPolicyDetails 资源类型
description: 加密策略详细信息报告
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 84a5f10542db3f2677cda68923eebf1bc2fb4008bfb0ee6a2669fd8be33f6951
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54241964"
---
# <a name="encryptionreportpolicydetails-resource-type"></a>encryptionReportPolicyDetails 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

加密策略详细信息报告

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|policyId|字符串|加密策略 ID 报告|
|policyName|String|加密策略名称报告|

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




