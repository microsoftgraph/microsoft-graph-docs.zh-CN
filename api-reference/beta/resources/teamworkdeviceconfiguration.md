---
title: teamworkDeviceConfiguration 资源类型
description: 表示已启用Microsoft Teams设备的配置详细信息。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8d913040b86bbb1b2e669bbbcb0d622326603ef5
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262331"
---
# <a name="teamworkdeviceconfiguration-resource-type"></a>teamworkDeviceConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示启用 Microsoft Teams 的设备的配置详细信息，包括软件版本、外围设备[](../resources/teamworkdevice.md)配置 (例如相机、显示器、麦克风和扬声器) 、硬件配置和 Teams 客户端配置。


继承自 [实体](../resources/entity.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 teamworkDeviceConfiguration](../api/teamworkdeviceconfiguration-get.md)|[teamworkDeviceConfiguration](../resources/teamworkdeviceconfiguration.md)|读取 [teamworkDeviceConfiguration](../resources/teamworkdeviceconfiguration.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|cameraConfiguration|[teamworkCameraConfiguration](../resources/teamworkcameraconfiguration.md)|相机配置。 仅适用于Microsoft Teams 会议室的设备。|
|createdBy|[identitySet](../resources/identityset.md)|创建设备配置文档的用户的标识。|
|createdDateTime|DateTimeOffset|创建设备配置文档的 UTC 日期和时间。|
|displayConfiguration|[teamworkDisplayConfiguration](../resources/teamworkdisplayconfiguration.md)|显示配置。|
|hardwareConfiguration|[teamworkHardwareConfiguration](../resources/teamworkhardwareconfiguration.md)|硬件配置。 仅适用于Teams 会议室的设备。|
|id|String|文档标识符。 继承自 [实体](../resources/entity.md)。|
|lastModifiedBy|[identitySet](../resources/identityset.md)|上次修改设备配置的用户的标识。|
|lastModifiedDateTime|DateTimeOffset|上次修改设备配置的 UTC 日期和时间。|
|microphoneConfiguration|[teamworkMicrophoneConfiguration](../resources/teamworkmicrophoneconfiguration.md)|麦克风配置。 仅适用于Teams 会议室的设备。|
|softwareVersions|[teamworkDeviceSoftwareVersions](../resources/teamworkdevicesoftwareversions.md)|与设备软件版本（如固件、操作系统、Teams客户端和管理代理）有关的信息。|
|speakerConfiguration|[teamworkSpeakerConfiguration](../resources/teamworkspeakerconfiguration.md)|扬声器配置。 仅适用于Teams 会议室的设备。|
|systemConfiguration|[teamworkSystemConfiguration](../resources/teamworksystemconfiguration.md)|系统配置。 不适用于Teams 会议室的设备。|
|teamsClientConfiguration|[teamworkTeamsClientConfiguration](../resources/teamworkteamsclientconfiguration.md)|客户端Teams配置。 仅适用于Teams 会议室的设备。|


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkDeviceConfiguration",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkDeviceConfiguration",
  "cameraConfiguration": {
    "@odata.type": "microsoft.graph.teamworkCameraConfiguration"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "displayConfiguration": {
    "@odata.type": "microsoft.graph.teamworkDisplayConfiguration"
  },
  "hardwareConfiguration": {
    "@odata.type": "microsoft.graph.teamworkHardwareConfiguration"
  },
  "id": "String (identifier)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "microphoneConfiguration": {
    "@odata.type": "microsoft.graph.teamworkMicrophoneConfiguration"
  },
  "softwareVersions": {
    "@odata.type": "microsoft.graph.teamworkDeviceSoftwareVersions"
  },
  "speakerConfiguration": {
    "@odata.type": "microsoft.graph.teamworkSpeakerConfiguration"
  },
  "systemConfiguration": {
    "@odata.type": "microsoft.graph.teamworkSystemConfiguration"
  },
  "teamsClientConfiguration": {
    "@odata.type": "microsoft.graph.teamworkTeamsClientConfiguration"
  }
}
```

