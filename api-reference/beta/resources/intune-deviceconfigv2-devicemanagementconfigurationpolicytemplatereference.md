---
title: deviceManagementConfigurationPolicyTemplateReference 资源类型
description: 策略模板参考信息
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ff61ac1e881ec6bb40750d9cb43d80c6722dd79e
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666497"
---
# <a name="devicemanagementconfigurationpolicytemplatereference-resource-type"></a>deviceManagementConfigurationPolicyTemplateReference 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

策略模板参考信息

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|templateId|String|模板 ID|
|templateFamily|[deviceManagementConfigurationTemplateFamily](../resources/intune-deviceconfigv2-devicemanagementconfigurationtemplatefamily.md)|引用的模板的模板系列。 此属性是只读的。 可取值为：`none`、`endpointSecurityAntivirus`、`endpointSecurityDiskEncryption`、`endpointSecurityFirewall`、`endpointSecurityEndpointDetectionAndResponse`、`endpointSecurityAttackSurfaceReduction`、`endpointSecurityAccountProtection`、`endpointSecurityApplicationControl`。|
|templateDisplayName|String|模板显示 引用的模板的名称。 此属性是只读的。|
|templateDisplayVersion|String|模板显示 引用的模板的版本。 此属性是只读的。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationPolicyTemplateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyTemplateReference",
  "templateId": "String",
  "templateFamily": "String",
  "templateDisplayName": "String",
  "templateDisplayVersion": "String"
}
```




