---
title: deviceManagementApplicabilityRuleOsVersion 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 505c57cb0ce7044344d13917bf420225637e2f74
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58804552"
---
# <a name="devicemanagementapplicabilityruleosversion-resource-type"></a>deviceManagementApplicabilityRuleOsVersion 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|minOSVersion|String|适用性规则最低操作系统版本。|
|maxOSVersion|String|适用性规则的最大操作系统版本。|
|name|String|对象的名称。|
|ruleType|[deviceManagementApplicabilityRuleType](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|适用性规则类型。 可取值为：`include`、`exclude`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
  "minOSVersion": "String",
  "maxOSVersion": "String",
  "name": "String",
  "ruleType": "String"
}
```



