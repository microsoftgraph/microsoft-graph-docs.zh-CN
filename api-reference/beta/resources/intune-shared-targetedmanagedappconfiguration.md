---
title: targetedManagedAppConfiguration 资源类型
description: 用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4807c7a0e9bde2ba3a6af12a0b603803a02c4936
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66438505"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a>targetedManagedAppConfiguration 资源类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于将一组自定义设置按原样提供给目标安全组中的所有用户的配置


继承自 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List targetedManagedAppConfigurations](../api/intune-shared-targetedmanagedappconfiguration-list.md)|[targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 集合|列出 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象的属性和关系。|
|[Get targetedManagedAppConfiguration](../api/intune-shared-targetedmanagedappconfiguration-get.md)|[targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md)|读取 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象的属性和关系。|
|[Create targetedManagedAppConfiguration](../api/intune-shared-targetedmanagedappconfiguration-create.md)|[targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md)|创建新的 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象。|
|[Delete targetedManagedAppConfiguration](../api/intune-shared-targetedmanagedappconfiguration-delete.md)|无|删除 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md)。|
|[Update targetedManagedAppConfiguration](../api/intune-shared-targetedmanagedappconfiguration-update.md)|[targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md)|更新 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象的属性。|
|**移动应用管理(MAM)**|
|[分配操作](../api/intune-shared-targetedmanagedappconfiguration-assign.md)|无|尚未记录|
|[targetApps 操作](../api/intune-shared-targetedmanagedappconfiguration-targetapps.md)|无|尚未记录|
|**策略集**|
|[hasPayloadLinks 操作](../api/intune-shared-targetedmanagedappconfiguration-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) 集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|displayName|String|策略显示名称。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|description|String|策略的说明。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|createdDateTime|DateTimeOffset|创建策略的日期和时间。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改策略的时间。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|version|String|实体的版本。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|customSettings|[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合|要发送到配置范围确定的用户应用的一组字符串键和字符串值对，不由此服务更改。继承自 [ managedAppConfiguration ](../resources/intune-mam-managedappconfiguration.md)|
|deployedAppCount|Int32|当前策略部署到的应用的计数。|
|isAssigned|Boolean|指示策略是否部署到任何包含组。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|**移动应用管理(MAM)**|
|apps|[managedMobileApp](../resources/intune-mam-managedmobileapp.md) 集合|策略部署到的应用的列表。|
|deploymentSummary|[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md)|配置的部署摘要的导航属性。|
|assignments|[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合|策略部署到的包含组和排除组列表的导航属性。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.targetedManagedAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "version": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "deployedAppCount": 1024,
  "isAssigned": true
}
```



