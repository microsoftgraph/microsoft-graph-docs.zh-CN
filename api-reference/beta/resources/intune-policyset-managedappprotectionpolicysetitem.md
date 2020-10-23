---
title: managedAppProtectionPolicySetItem 资源类型
description: 包含用于托管应用程序保护 PolicySetItem 的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e160e88c54e7cc8d33e0c78090fbf06dfd52cab1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736049"
---
# <a name="managedappprotectionpolicysetitem-resource-type"></a>managedAppProtectionPolicySetItem 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于托管应用程序保护 PolicySetItem 的属性的类。


继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 managedAppProtectionPolicySetItems](../api/intune-policyset-managedappprotectionpolicysetitem-list.md)|[managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) 集合|列出 [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) 对象的属性和关系。|
|[获取 managedAppProtectionPolicySetItem](../api/intune-policyset-managedappprotectionpolicysetitem-get.md)|[managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md)|读取 [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) 对象的属性和关系。|
|[创建 managedAppProtectionPolicySetItem](../api/intune-policyset-managedappprotectionpolicysetitem-create.md)|[managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md)|创建新的 [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) 对象。|
|[删除 managedAppProtectionPolicySetItem](../api/intune-policyset-managedappprotectionpolicysetitem-delete.md)|无|删除 [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md)。|
|[更新 managedAppProtectionPolicySetItem](../api/intune-policyset-managedappprotectionpolicysetitem-update.md)|[managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md)|更新 [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|MobileAppPolicySetItem 的键。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|createdDateTime|DateTimeOffset|PolicySetItem 的创建时间。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|lastModifiedDateTime|DateTimeOffset|PolicySetItem 的上次修改时间。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|payloadId|String|PolicySetItem 的 PayloadId。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|itemType|String|PolicySetItem 的 policySetType。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|displayName|String|PolicySetItem 的 DisplayName。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|status|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|PolicySetItem 的状态。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。 可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|错误代码（如果发生）。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。 可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。|
|guidedDeploymentTags|String collection|继承自[policySetItem](../resources/intune-policyset-policysetitem.md)的引导部署的标记|
|targetedAppManagementLevels|String|ManagedAppPolicySetItem 的 TargetedAppManagementLevels。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppProtectionPolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppProtectionPolicySetItem",
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
  "targetedAppManagementLevels": "String"
}
```





