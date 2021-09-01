---
title: deviceManagementConfigurationPolicyPolicySetItem 资源类型
description: 包含用于 DeviceManagementConfiguration PolicySetItem 的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b8b7136c06822cfe1f54c1ac601617a7edd1b331
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58800357"
---
# <a name="devicemanagementconfigurationpolicypolicysetitem-resource-type"></a>deviceManagementConfigurationPolicyPolicySetItem 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于 DeviceManagementConfiguration PolicySetItem 的属性的类。


继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementConfigurationPolicyPolicySetItems](../api/intune-policyset-devicemanagementconfigurationpolicypolicysetitem-list.md)|[deviceManagementConfigurationPolicyPolicySetItem](../resources/intune-policyset-devicemanagementconfigurationpolicypolicysetitem.md) 集合|列出 [deviceManagementConfigurationPolicyPolicySetItem 对象的属性和](../resources/intune-policyset-devicemanagementconfigurationpolicypolicysetitem.md) 关系。|
|[获取 deviceManagementConfigurationPolicyPolicySetItem](../api/intune-policyset-devicemanagementconfigurationpolicypolicysetitem-get.md)|[deviceManagementConfigurationPolicyPolicySetItem](../resources/intune-policyset-devicemanagementconfigurationpolicypolicysetitem.md)|读取 [deviceManagementConfigurationPolicyPolicySetItem 对象的属性和](../resources/intune-policyset-devicemanagementconfigurationpolicypolicysetitem.md) 关系。|
|[创建 deviceManagementConfigurationPolicyPolicySetItem](../api/intune-policyset-devicemanagementconfigurationpolicypolicysetitem-create.md)|[deviceManagementConfigurationPolicyPolicySetItem](../resources/intune-policyset-devicemanagementconfigurationpolicypolicysetitem.md)|创建新的 [deviceManagementConfigurationPolicyPolicySetItem](../resources/intune-policyset-devicemanagementconfigurationpolicypolicysetitem.md) 对象。|
|[删除 deviceManagementConfigurationPolicyPolicySetItem](../api/intune-policyset-devicemanagementconfigurationpolicypolicysetitem-delete.md)|无|删除 [deviceManagementConfigurationPolicyPolicySetItem](../resources/intune-policyset-devicemanagementconfigurationpolicypolicysetitem.md)。|
|[更新 deviceManagementConfigurationPolicyPolicySetItem](../api/intune-policyset-devicemanagementconfigurationpolicypolicysetitem-update.md)|[deviceManagementConfigurationPolicyPolicySetItem](../resources/intune-policyset-devicemanagementconfigurationpolicypolicysetitem.md)|更新 [deviceManagementConfigurationPolicyPolicySetItem 对象](../resources/intune-policyset-devicemanagementconfigurationpolicypolicysetitem.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|PolicySetItem 的键。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|createdDateTime|DateTimeOffset|PolicySetItem 的创建时间。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|lastModifiedDateTime|DateTimeOffset|PolicySetItem 的上次修改时间。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|payloadId|String|PolicySetItem 的 PayloadId。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|itemType|String|PolicySetItem 的 policySetType。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|displayName|字符串|PolicySetItem 的 DisplayName。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|状态|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|PolicySetItem 的状态。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。 可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|错误代码（如果发生了任何错误）。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。 可能的值是：`noError`、`unauthorized`、`notFound`、`deleted`。|
|guidedDeploymentTags|字符串集合|引导式部署的标记 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationPolicyPolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyPolicySetItem",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "payloadId": "String",
  "itemType": "String",
  "displayName": "String",
  "status": "String",
  "errorCode": "String",
  "guidedDeploymentTags": [
    "String"
  ]
}
```



