---
title: deviceConfigurationTargetedUserAndDevice 资源类型
description: 一组设备配置策略的冲突摘要。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 84657d0401025473cc2f5628672eb413d3ac7ba4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59051396"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a>deviceConfigurationTargetedUserAndDevice 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

一组设备配置策略的冲突摘要。

## <a name="properties"></a>属性
|属性|类型|说明|
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



