---
title: deviceConfigurationTargetedUserAndDevice 资源类型
description: 一组设备配置策略的冲突摘要。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 637d86c32dd00fdb30cae205cd85484b729925d3
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58819183"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a>deviceConfigurationTargetedUserAndDevice 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

一组设备配置策略的冲突摘要。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|deviceId|String|签入中的设备的 ID。|
|deviceName|String|签入中的设备名称。|
|userId|String|签入中的用户 ID。|
|userDisplayName|String|显示名称签入中的用户权限|
|userPrincipalName|String|签入中的用户的 UPN。|
|lastCheckinDateTime|DateTimeOffset|此用户/设备对的上次签入时间。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationTargetedUserAndDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationTargetedUserAndDevice",
  "deviceId": "String",
  "deviceName": "String",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "lastCheckinDateTime": "String (timestamp)"
}
```



