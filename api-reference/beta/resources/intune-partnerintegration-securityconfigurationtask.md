---
title: securityConfigurationTask 资源类型
description: 安全配置任务。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: eaf2f479d491e8d6455dc3b296053a84983fdf98
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46793229"
---
# <a name="securityconfigurationtask-resource-type"></a>securityConfigurationTask 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

安全配置任务。


继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 securityConfigurationTasks](../api/intune-partnerintegration-securityconfigurationtask-list.md)|[securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) 集合|列出 [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) 对象的属性和关系。|
|[获取 securityConfigurationTask](../api/intune-partnerintegration-securityconfigurationtask-get.md)|[securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md)|读取 [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) 对象的属性和关系。|
|[创建 securityConfigurationTask](../api/intune-partnerintegration-securityconfigurationtask-create.md)|[securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md)|创建新的 [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) 对象。|
|[删除 securityConfigurationTask](../api/intune-partnerintegration-securityconfigurationtask-delete.md)|无|删除 [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md)。|
|[更新 securityConfigurationTask](../api/intune-partnerintegration-securityconfigurationtask-update.md)|[securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md)|更新 [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体键。 继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|displayName|String|名称。 继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|description|String|说明。 继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|createdDateTime|DateTimeOffset|创建日期。 继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|dueDateTime|DateTimeOffset|到期日期。 继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|“类别”|[deviceAppManagementTaskCategory](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|类别。 继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)。 可取值为：`unknown`、`advancedThreatProtection`。|
|priority|[deviceAppManagementTaskPriority](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|优先级。 继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)。 可取值为：`none`、`high`、`low`。|
|创建|String|创建者的电子邮件地址。 继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|creatorNotes|String|来自创建者的注释。 继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|assignedTo|String|将此任务分配到的管理员的姓名或电子邮件。 继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|status|[deviceAppManagementTaskStatus](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|状态。 继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)。 可取值为：`unknown`、`pending`、`active`、`completed`、`rejected`。|
|endpointSecurityPolicy|[endpointSecurityConfigurationType](../resources/intune-partnerintegration-endpointsecurityconfigurationtype.md)|终结点安全策略类型。 可取值为：`unknown`、`antivirus`、`diskEncryption`、`firewall`、`endpointDetectionAndResponse`、`attackSurfaceReduction` 或 `accountProtection`。|
|applicablePlatform|[endpointSecurityConfigurationApplicablePlatform](../resources/intune-partnerintegration-endpointsecurityconfigurationapplicableplatform.md)|适用的平台。 可取值为：`unknown`、`macOS`、`windows10AndLater`、`windows10AndWindowsServer`。|
|endpointSecurityPolicyProfile|[endpointSecurityConfigurationProfileType](../resources/intune-partnerintegration-endpointsecurityconfigurationprofiletype.md)|终结点安全策略配置文件。 可能的值为：、、、、、、、、、、、、、、 `unknown` `antivirus` `windowsSecurity` `bitLocker` `fileVault` `firewall` `firewallRules` `endpointDetectionAndResponse` `deviceControl` `appAndBrowserIsolation` `exploitProtection` `webProtection` `applicationControl` `attackSurfaceReductionRules` `accountProtection` 。|
|insights|String|有关缓解措施的信息。|
|managedDeviceCount|Int32|易受攻击设备的数量。|
|intendedSettings|[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合|预期的设置及其值。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|managedDevices|[vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) 集合|易受攻击的托管设备。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityConfigurationTask"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityConfigurationTask",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "dueDateTime": "String (timestamp)",
  "category": "String",
  "priority": "String",
  "creator": "String",
  "creatorNotes": "String",
  "assignedTo": "String",
  "status": "String",
  "endpointSecurityPolicy": "String",
  "applicablePlatform": "String",
  "endpointSecurityPolicyProfile": "String",
  "insights": "String",
  "managedDeviceCount": 1024,
  "intendedSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```



