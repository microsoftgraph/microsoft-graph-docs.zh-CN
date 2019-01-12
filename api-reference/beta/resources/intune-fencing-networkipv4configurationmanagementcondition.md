---
title: networkIPv4ConfigurationManagementCondition 资源类型
description: 配置基于管理条件可能定义设备检测到某些 IP 时将触发的 IPv4 网络设置。 IP 配置管理条件仅被视为 TRUE 的网络连接处于活动状态时。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 412f5de452e23eeb58f536655c4678526e996e07
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962105"
---
# <a name="networkipv4configurationmanagementcondition-resource-type"></a>networkIPv4ConfigurationManagementCondition 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

配置基于管理条件可能定义设备检测到某些 IP 时将触发的 IPv4 网络设置。 IP 配置管理条件仅被视为 TRUE 的网络连接处于活动状态时。

继承自[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 networkIPv4ConfigurationManagementConditions](../api/intune-fencing-networkipv4configurationmanagementcondition-list.md)|[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)集合|列出属性和[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)对象之间的关系。|
|[获取 networkIPv4ConfigurationManagementCondition](../api/intune-fencing-networkipv4configurationmanagementcondition-get.md)|[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)|读取属性和[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)对象的关系。|
|[创建 networkIPv4ConfigurationManagementCondition](../api/intune-fencing-networkipv4configurationmanagementcondition-create.md)|[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)|创建新的[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)对象。|
|[删除 networkIPv4ConfigurationManagementCondition](../api/intune-fencing-networkipv4configurationmanagementcondition-delete.md)|无|删除[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)。|
|[更新 networkIPv4ConfigurationManagementCondition](../api/intune-fencing-networkipv4configurationmanagementcondition-update.md)|[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)|更新[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|管理条件的唯一标识符。 系统生成时创建分配值。 继承自[managementCondition](../resources/intune-fencing-managementcondition.md)|
|唯一名称|字符串|管理条件的唯一名称。 在管理条件表达式中使用。 继承自[managementCondition](../resources/intune-fencing-managementcondition.md)|
|displayName|字符串|管理员定义管理条件的名称。 继承自[managementCondition](../resources/intune-fencing-managementcondition.md)|
|说明|字符串|管理员定义的管理条件说明。 继承自[managementCondition](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|创建管理条件的时间。 生成的服务方。 继承自[managementCondition](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|管理条件上次修改时间。 更新服务端。 继承自[managementCondition](../resources/intune-fencing-managementcondition.md)|
|eTag|String|管理条件的 ETag。 更新服务端。 继承自[managementCondition](../resources/intune-fencing-managementcondition.md)|
|applicablePlatforms|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合|此管理条件适用的平台。 继承自[managementCondition](../resources/intune-fencing-managementcondition.md)|
|ipV4Prefix|字符串|要连接到的 IPv4 子网。 例如 10.0.0.0/8|
|ipV4Gateway|字符串|IPv4 网关地址。 例如 10.0.0.0|
|ipV4DHCPServer|字符串|为此适配器 DHCP 服务器的 IPv4 地址。|
|ipV4DNSServerList|String 集合|配置为此适配器 IPv4 DNS 服务器。|
|dnsSuffixList|String 集合|当前网络的有效 DNS 后缀。 例如 seattle.contoso.com|

## <a name="relationships"></a>Relationships
|关系|类型|Description|
|:---|:---|:---|
|managementConditionStatements|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)集合|为管理 condition 相关联的管理条件语句。 继承自[managementCondition](../resources/intune-fencing-managementcondition.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.networkIPv4ConfigurationManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ],
  "ipV4Prefix": "String",
  "ipV4Gateway": "String",
  "ipV4DHCPServer": "String",
  "ipV4DNSServerList": [
    "String"
  ],
  "dnsSuffixList": [
    "String"
  ]
}
```





