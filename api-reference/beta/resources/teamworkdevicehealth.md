---
title: teamworkDeviceHealth 资源类型
description: 表示已启用Microsoft Teams的设备的运行状况详细信息。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0c26b784f42dedc87b02e3a616ff93b7f0c1b46b
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262324"
---
# <a name="teamworkdevicehealth-resource-type"></a>teamworkDeviceHealth 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示已启用Microsoft Teams的设备的运行状况[详细信息](../resources/teamworkdevice.md)。 根据设备配置和其他设备参数计算设备运行状况。

继承自 [实体](../resources/entity.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 teamworkDeviceHealth](../api/teamworkdevicehealth-get.md)|[teamworkDeviceHealth](../resources/teamworkdevicehealth.md)|读取 [teamworkDeviceHealth 对象的属性和](../resources/teamworkdevicehealth.md) 关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|connection|[teamworkConnection](../resources/teamworkconnection.md)|有关连接状态的信息。|
|createdBy|[identitySet](../resources/identityset.md)|创建设备运行状况文档的用户的标识。|
|createdDateTime|DateTimeOffset|创建设备运行状况文档的 UTC 日期和时间。|
|hardwareHealth|[teamworkHardwareHealth](../resources/teamworkhardwarehealth.md)|有关设备硬件的运行状况详细信息。|
|id|String|Doucument 标识符。 继承自 [实体](../resources/entity.md)。|
|lastModifiedBy|[identitySet](../resources/identityset.md)|上次修改设备运行状况详细信息的用户的标识。|
|lastModifiedDateTime|DateTimeOffset|上次修改设备运行状况详细信息的 UTC 日期和时间。|
|loginStatus|[teamworkLoginStatus](../resources/teamworkloginstatus.md)|Microsoft Teams、Skype for Business 和 Exchange 的登录Exchange。|
|peripheralsHealth|[teamworkPeripheralsHealth](../resources/teamworkperipheralshealth.md)|有关所有外围设备的运行状况 (例如，扬声器和麦克风) 设备。|
|softwareUpdateHealth|[teamworkSoftwareUpdateHealth](../resources/teamworksoftwareupdatehealth.md)|设备可用的软件更新。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkDeviceHealth",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkDeviceHealth",
  "connection": {
    "@odata.type": "microsoft.graph.teamworkConnection"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "hardwareHealth": {
    "@odata.type": "microsoft.graph.teamworkHardwareHealth"
  },
  "id": "String (identifier)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "loginStatus": {
    "@odata.type": "microsoft.graph.teamworkLoginStatus"
  },
  "peripheralsHealth": {
    "@odata.type": "microsoft.graph.teamworkPeripheralsHealth"
  },
  "softwareUpdateHealth": {
    "@odata.type": "microsoft.graph.teamworkSoftwareUpdateHealth"
  }
}
```

