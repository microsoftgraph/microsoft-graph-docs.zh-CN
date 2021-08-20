---
title: deviceManagementApplicabilityRuleOsEdition 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 044c43dce614c27a3ff408dfa67692bee638614af86bbd5aadeef58faa3da737
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54242949"
---
# <a name="devicemanagementapplicabilityruleosedition-resource-type"></a>deviceManagementApplicabilityRuleOsEdition 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|osEditionTypes|[windows10EditionType](../resources/intune-deviceconfig-windows10editiontype.md) 集合|适用性规则 OS 版本类型。|
|name|String|对象的名称。|
|ruleType|[deviceManagementApplicabilityRuleType](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|适用性规则类型。 可取值为：`include`、`exclude`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
  "osEditionTypes": [
    "String"
  ],
  "name": "String",
  "ruleType": "String"
}
```




