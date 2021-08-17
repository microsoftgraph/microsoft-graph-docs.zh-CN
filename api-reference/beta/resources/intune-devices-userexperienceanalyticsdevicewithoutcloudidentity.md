---
title: userExperienceAnalyticsDeviceWithoutCloudIdentity 资源类型
description: 用户体验分析设备（无云标识）。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0a6560696ccce4360c33fce65bb83b8a78d25f92b022677761cf2a51fa0fde56
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54126917"
---
# <a name="userexperienceanalyticsdevicewithoutcloudidentity-resource-type"></a>userExperienceAnalyticsDeviceWithoutCloudIdentity 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析设备（无云标识）。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsDeviceWithoutCloudIdentities](../api/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity-list.md)|[userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md) 集合|列出 [userExperienceAnalyticsDeviceWithoutCloudIdentity 对象的属性和](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md) 关系。|
|[获取 userExperienceAnalyticsDeviceWithoutCloudIdentity](../api/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity-get.md)|[userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md)|读取 [userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md) 对象的属性和关系。|
|[创建 userExperienceAnalyticsDeviceWithoutCloudIdentity](../api/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity-create.md)|[userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md)|创建新的 [userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md) 对象。|
|[删除 userExperienceAnalyticsDeviceWithoutCloudIdentity](../api/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity-delete.md)|无|删除 [userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md)。|
|[更新 userExperienceAnalyticsDeviceWithoutCloudIdentity](../api/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity-update.md)|[userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md)|更新 [userExperienceAnalyticsDeviceWithoutCloudIdentity 对象](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析租户附加设备的唯一标识符。|
|deviceName|String|租户附加设备的名称。|
|azureAdDeviceId|String|Azure Active Directory设备 ID|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsDeviceWithoutCloudIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceWithoutCloudIdentity",
  "id": "String (identifier)",
  "deviceName": "String",
  "azureAdDeviceId": "String"
}
```




