---
title: networkIPv6ConfigurationManagementCondition 资源类型
description: 可以定义基于 IPv6 配置的管理条件，当设备检测到某些 IP 网络设置时将触发这些条件。 只有在网络连接处于活动状态时，IP 配置管理条件才被视为 TRUE。 IPv6 DHCP 服务器地址可能不匹配。 这是因为，Windows (Redstone) 不会向自然身份验证服务公开此信息。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bf74b6a655244e3ed7422ea1f9201f1dbe2f958e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59063946"
---
# <a name="networkipv6configurationmanagementcondition-resource-type"></a>networkIPv6ConfigurationManagementCondition 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

可以定义基于 IPv6 配置的管理条件，当设备检测到某些 IP 网络设置时将触发这些条件。 只有在网络连接处于活动状态时，IP 配置管理条件才被视为 TRUE。
IPv6 DHCP 服务器地址可能不匹配。 这是因为，Windows (Redstone) 不会向自然身份验证服务公开此信息。


继承自 [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 networkIPv6ConfigurationManagementConditions](../api/intune-fencing-networkipv6configurationmanagementcondition-list.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) 集合|列出 [networkIPv6ConfigurationManagementCondition 对象的属性和](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) 关系。|
|[获取 networkIPv6ConfigurationManagementCondition](../api/intune-fencing-networkipv6configurationmanagementcondition-get.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|读取 [networkIPv6ConfigurationManagementCondition 对象的属性和](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) 关系。|
|[创建 networkIPv6ConfigurationManagementCondition](../api/intune-fencing-networkipv6configurationmanagementcondition-create.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|创建新的 [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) 对象。|
|[删除 networkIPv6ConfigurationManagementCondition](../api/intune-fencing-networkipv6configurationmanagementcondition-delete.md)|无|删除 [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)。|
|[更新 networkIPv6ConfigurationManagementCondition](../api/intune-fencing-networkipv6configurationmanagementcondition-update.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|更新 [networkIPv6ConfigurationManagementCondition 对象](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|管理条件的唯一标识符。 创建时分配的系统生成值。 继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)|
|唯一名称|String|管理条件的唯一名称。 在管理条件表达式中使用。 继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)|
|displayName|String|管理员定义的管理条件名称。 继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)|
|说明|String|管理员定义的管理条件说明。 继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|创建管理条件的时间。 生成的服务器端。 继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|上次修改管理条件的时间。 更新的服务器端。 继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)|
|eTag|String|管理条件的 ETag。 更新的服务器端。 继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)|
|applicablePlatforms|[devicePlatformType](../resources/intune-fencing-deviceplatformtype.md) 集合|此管理条件的适用平台。 继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)|
|ipV6Prefix|String|要连接到的 IPv6 子网。 例如 2001：db8：：/32|
|ipV6Gateway|String|IPv6 网关地址。 例如 2001：db8：：1|
|ipV6DNSServerList|String collection|为适配器配置的 IPv6 DNS 服务器。|
|dnsSuffixList|String collection|当前网络的有效 DNS 后缀。 例如 seattle.contoso.com|

## <a name="relationships"></a>关系
|关系|类型|描述|
|:---|:---|:---|
|managementConditionStatements|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) 集合|与管理条件关联的管理条件语句。 继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.networkIPv6ConfigurationManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
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
  "ipV6Prefix": "String",
  "ipV6Gateway": "String",
  "ipV6DNSServerList": [
    "String"
  ],
  "dnsSuffixList": [
    "String"
  ]
}
```



