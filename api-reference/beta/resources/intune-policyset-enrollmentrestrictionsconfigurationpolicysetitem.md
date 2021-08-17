---
title: enrollmentRestrictionsConfigurationPolicySetItem 资源类型
description: 包含用于注册限制 PolicySetItem 的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d94a4099e26410044c887bd1e49f395210ba70cb
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58262177"
---
# <a name="enrollmentrestrictionsconfigurationpolicysetitem-resource-type"></a>enrollmentRestrictionsConfigurationPolicySetItem 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于注册限制 PolicySetItem 的属性的类。


继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 enrollmentRestrictionsConfigurationPolicySetItems](../api/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem-list.md)|[enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) 集合|列出 [enrollmentRestrictionsConfigurationPolicySetItem 对象的属性和](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) 关系。|
|[获取 enrollmentRestrictionsConfigurationPolicySetItem](../api/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem-get.md)|[enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)|读取 [enrollmentRestrictionsConfigurationPolicySetItem 对象的属性和](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) 关系。|
|[创建 enrollmentRestrictionsConfigurationPolicySetItem](../api/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem-create.md)|[enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)|创建新的 [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) 对象。|
|[删除 enrollmentRestrictionsConfigurationPolicySetItem](../api/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem-delete.md)|无|删除 [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)。|
|[更新 enrollmentRestrictionsConfigurationPolicySetItem](../api/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem-update.md)|[enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md)|更新 [enrollmentRestrictionsConfigurationPolicySetItem 对象](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|PolicySetItem 的键。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|createdDateTime|DateTimeOffset|PolicySetItem 的创建时间。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|lastModifiedDateTime|DateTimeOffset|PolicySetItem 的上次修改时间。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|payloadId|String|PolicySetItem 的 PayloadId。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|itemType|String|PolicySetItem 的 policySetType。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|displayName|字符串|PolicySetItem 的 DisplayName。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|status|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|PolicySetItem 的状态。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。 可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|错误代码（如果发生了任何错误）。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。 可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。|
|guidedDeploymentTags|String collection|引导式部署的标记 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|priority|Int32|EnrollmentRestrictionsConfigurationPolicySetItem 的优先级。|
|limit|Int32|EnrollmentRestrictionsConfigurationPolicySetItem 的限制。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentRestrictionsConfigurationPolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentRestrictionsConfigurationPolicySetItem",
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
  ],
  "priority": 1024,
  "limit": 1024
}
```




