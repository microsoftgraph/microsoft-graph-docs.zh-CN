---
title: userExperienceAnalyticsRemoteConnection 资源类型
description: 用户体验分析远程连接实体。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 62d6d012e94a0423b3951d1345704d4447b81e1f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59020348"
---
# <a name="userexperienceanalyticsremoteconnection-resource-type"></a>userExperienceAnalyticsRemoteConnection 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析远程连接实体。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsRemoteConnections](../api/intune-devices-userexperienceanalyticsremoteconnection-list.md)|[userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) 集合|列出 [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) 对象的属性和关系。|
|[获取 userExperienceAnalyticsRemoteConnection](../api/intune-devices-userexperienceanalyticsremoteconnection-get.md)|[userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)|读取 [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) 对象的属性和关系。|
|[创建 userExperienceAnalyticsRemoteConnection](../api/intune-devices-userexperienceanalyticsremoteconnection-create.md)|[userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)|创建新的 [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) 对象。|
|[删除 userExperienceAnalyticsRemoteConnection](../api/intune-devices-userexperienceanalyticsremoteconnection-delete.md)|无|删除 [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)。|
|[更新 userExperienceAnalyticsRemoteConnection](../api/intune-devices-userexperienceanalyticsremoteconnection-update.md)|[userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)|更新 [userExperienceAnalyticsRemoteConnection 对象](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) 的属性。|
|[summarizeDeviceRemoteConnection 函数](../api/intune-devices-userexperienceanalyticsremoteconnection-summarizedeviceremoteconnection.md)|[userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) 集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析远程连接实体的唯一标识符。|
|deviceId|String|设备的 ID。|
|deviceName|String|设备的名称。|
|model|String|用户体验分析设备模型。|
|virtualNetwork|String|用户体验分析虚拟网络。|
|manufacturer|String|用户体验分析制造商。|
|deviceCount|Int32|远程连接计数。 有效值为 0 到 2147483647|
|cloudPcRoundTripTime|双精度|云电脑设备的舍入提示时间。 有效值为 0 到 1.79769313486232E+308|
|cloudPcSignInTime|双精度|云电脑设备的登录时间。 有效值为 0 到 1.79769313486232E+308|
|remoteSignInTime|双精度|云电脑设备的远程登录时间。 有效值为 0 到 1.79769313486232E+308|
|coreBootTime|双精度|云电脑设备的核心启动时间。 有效值为 0 到 1.79769313486232E+308|
|coreSignInTime|双精度|云电脑设备的核心登录时间。 有效值为 0 到 1.79769313486232E+308|
|cloudPcFailurePercentage|双精度|云电脑设备的登录失败百分比。 有效值为 0 至 100|
|userPrincipalName|String|用户体验分析 userPrincipalName。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsRemoteConnection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRemoteConnection",
  "id": "String (identifier)",
  "deviceId": "String",
  "deviceName": "String",
  "model": "String",
  "virtualNetwork": "String",
  "manufacturer": "String",
  "deviceCount": 1024,
  "cloudPcRoundTripTime": "4.2",
  "cloudPcSignInTime": "4.2",
  "remoteSignInTime": "4.2",
  "coreBootTime": "4.2",
  "coreSignInTime": "4.2",
  "cloudPcFailurePercentage": "4.2",
  "userPrincipalName": "String"
}
```



