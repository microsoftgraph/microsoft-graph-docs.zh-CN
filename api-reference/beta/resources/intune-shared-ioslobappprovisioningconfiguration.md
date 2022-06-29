---
title: iosLobAppProvisioningConfiguration 资源类型
description: 本主题提供 iOS Lob 应用预配配置资源公开的已声明方法、属性和关系的说明。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b755ab6a94bca06b2ba73f2d896dc3a382077b1e
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439940"
---
# <a name="ioslobappprovisioningconfiguration-resource-type"></a>iosLobAppProvisioningConfiguration 资源类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

本主题提供 iOS Lob 应用预配配置资源公开的已声明方法、属性和关系的说明。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 iosLobAppProvisioningConfigurations](../api/intune-shared-ioslobappprovisioningconfiguration-list.md)|[iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) 集合|列出 [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) 对象的属性和关系。|
|[获取 iosLobAppProvisioningConfiguration](../api/intune-shared-ioslobappprovisioningconfiguration-get.md)|[iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)|读取 [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) 对象的属性和关系。|
|[创建 iosLobAppProvisioningConfiguration](../api/intune-shared-ioslobappprovisioningconfiguration-create.md)|[iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)|创建新的 [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) 对象。|
|[删除 iosLobAppProvisioningConfiguration](../api/intune-shared-ioslobappprovisioningconfiguration-delete.md)|无|删除 [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)。|
|[更新 iosLobAppProvisioningConfiguration](../api/intune-shared-ioslobappprovisioningconfiguration-update.md)|[iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)|更新 [iosLobAppProvisioningConfiguration 对象的](../resources/intune-shared-ioslobappprovisioningconfiguration.md) 属性。|
|**应用**|
|[分配操作](../api/intune-shared-ioslobappprovisioningconfiguration-assign.md)|无|尚未记录|
|**策略集**|
|[hasPayloadLinks 操作](../api/intune-shared-ioslobappprovisioningconfiguration-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) 集合|尚未记录|

## <a name="properties"></a>属性
| 属性 | 类型 | 说明 |
| --- | --- | --- |
|id|String|实体的键。|
|expirationDateTime|DateTimeOffset|可选配置文件过期日期和时间。|
|payloadFileName|String|有效负载文件名 (*.mobileprovision | *.xml)。|
|payload|Binary|有效负载。 （UTF8 编码的字节数组）|
|roleScopeTagIds|字符串集合|此 iOS LOB 应用预配配置实体的作用域标记列表。|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。|
|description|String|管理员提供的设备配置说明。|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。|
|displayName|String|管理员提供的设备配置名称。|
|version|Int32|设备配置的版本。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|**应用**|
|groupAssignments|[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) 集合|关联的组分配。|
|assignments|[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) 集合|IosLobAppProvisioningConfiguration 的关联组分配。|
|deviceStatuses|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) 集合|此移动应用配置的设备安装状态列表。|
|userStatuses|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) 集合|此移动应用配置的用户安装状态列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosLobAppProvisioningConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "id": "String (identifier)",
  "expirationDateTime": "String (timestamp)",
  "payloadFileName": "String",
  "payload": "binary",
  "roleScopeTagIds": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```



