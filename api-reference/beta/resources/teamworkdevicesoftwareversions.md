---
title: teamworkDeviceSoftwareVersions 资源类型
description: 表示有关启用了移动设备的Microsoft Teams的详细信息。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0605b526e6e3fb3536d1a2fb7c2c14430a8309ed
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262310"
---
# <a name="teamworkdevicesoftwareversions-resource-type"></a>teamworkDeviceSoftwareVersions 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关启用了 [Microsoft Teams 的设备（](../resources/teamworkdevice.md)包括固件、操作系统、Microsoft Teams客户端和管理代理）的软件版本的详细信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|adminAgentSoftwareVersion|String|设备上运行的管理员代理的软件版本。|
|firmwareSoftwareVersion|String|设备上运行的固件的软件版本。|
|operatingSystemSoftwareVersion|字符串|设备上操作系统的软件版本。|
|partnerAgentSoftwareVersion|String|设备上运行的合作伙伴代理的软件版本。|
|teamsClientSoftwareVersion|String|设备上运行的 Teams 客户端的软件版本。|


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkDeviceSoftwareVersions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkDeviceSoftwareVersions",
  "adminAgentSoftwareVersion": "String",
  "firmwareSoftwareVersion": "String",
  "operatingSystemSoftwareVersion": "String",
  "partnerAgentSoftwareVersion": "String",
  "teamsClientSoftwareVersion": "String"
}
```

