---
title: windowsDomainJoinConfiguration 资源类型
description: Windows 域加入设备配置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 677185e0573d214d2ba53423bf741ae3b16dd5c4
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446341"
---
# <a name="windowsdomainjoinconfiguration-resource-type"></a>windowsDomainJoinConfiguration 资源类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows 域加入设备配置。

继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)

## <a name="methods"></a>方法
| 方法 | 返回类型 | 说明 |
| --- | --- | --- |
|[列出 windowsDomainJoinConfigurations](../api/intune-shared-windowsdomainjoinconfiguration-list.md)|[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) 集合|列出 [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) 对象的属性和关系。|
|[获取 windowsDomainJoinConfiguration](../api/intune-shared-windowsdomainjoinconfiguration-get.md)|[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)|读取 [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) 对象的属性和关系。|
|[创建 windowsDomainJoinConfiguration](../api/intune-shared-windowsdomainjoinconfiguration-create.md)|[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)|创建新的 [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) 对象。|
|[删除 windowsDomainJoinConfiguration](../api/intune-shared-windowsdomainjoinconfiguration-delete.md)|无|删除 [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)。|删除 [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) 对象。|
|[更新 windowsDomainJoinConfiguration](../api/intune-shared-windowsdomainjoinconfiguration-update.md)|[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)|更新 [windowsDomainJoinConfiguration 对象的](../resources/intune-shared-windowsdomainjoinconfiguration.md) 属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|**设备配置**|
|activeDirectoryDomainName|String|要加入的 Active Directory 域名。|
|computerNameStaticPrefix|String|修复了用于计算机名称的前缀。|
|computerNameSuffixRandomCharCount|Int32|动态生成的字符用作计算机名称的后缀。 有效值 3 到 14|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|description|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|organizationalUnit|String|组织单位 (要在其中创建计算机帐户的 OU) 。 如果此参数为 NULL，则已知计算机对象容器将用作域中发布的容器。|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Boolean|指示基础设备配置是否支持分配范围标记。 如果此值为 false，并且作用域内用户不可见，则不允许分配到 ScopeTags 属性。 对于在 Silverlight 中创建的旧策略，可以通过在 Azure 门户中删除和重新创建策略来解决此问题。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|**设备配置**|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合|设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合|按设备的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 集合|设备配置文件的组分配列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|networkAccessConfigurations|[deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) 集合|对网络连接所需的设备配置的引用|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合|按用户的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。  注意：为简洁起见，可能会截断此处显示的响应对象。 响应对象将包含与调用上下文相关的属性。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDomainJoinConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "computerNameStaticPrefix": "String",
  "computerNameSuffixRandomCharCount": 1024,
  "activeDirectoryDomainName": "String"
}
```



