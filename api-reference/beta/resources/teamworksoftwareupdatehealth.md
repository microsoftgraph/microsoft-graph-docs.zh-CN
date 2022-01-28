---
title: teamworkSoftwareUpdateHealth 资源类型
description: 表示有关可用于不同组件（如启用了 Microsoft Teams 的设备中的管理员代理、公司门户、固件、操作系统、合作伙伴代理和 Microsoft Teams 客户端）的详细信息。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8ac1ab4746c83bbcae613c723e1e38ba5f085b4e
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262344"
---
# <a name="teamworksoftwareupdatehealth-resource-type"></a>teamworkSoftwareUpdateHealth 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关可用于不同组件（如启用了 Microsoft Teams 的设备中的管理员代理、公司门户、固件、操作系统、合作伙伴代理和 Microsoft Teams 客户端）的软件更新[的详细信息](../resources/teamworkdevice.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|adminAgentSoftwareUpdateStatus|[teamworkSoftwareUpdateStatus](../resources/teamworksoftwareupdatestatus.md)|适用于管理员代理的软件更新。|
|companyPortalSoftwareUpdateStatus|[teamworkSoftwareUpdateStatus](../resources/teamworksoftwareupdatestatus.md)|可用于公司门户的软件更新。|
|firmwareSoftwareUpdateStatus|[teamworkSoftwareUpdateStatus](../resources/teamworksoftwareupdatestatus.md)|固件可用的软件更新。|
|operatingSystemSoftwareUpdateStatus|[teamworkSoftwareUpdateStatus](../resources/teamworksoftwareupdatestatus.md)|操作系统可用的软件更新。|
|partnerAgentSoftwareUpdateStatus|[teamworkSoftwareUpdateStatus](../resources/teamworksoftwareupdatestatus.md)|合作伙伴代理可用的软件更新。|
|teamsClientSoftwareUpdateStatus|[teamworkSoftwareUpdateStatus](../resources/teamworksoftwareupdatestatus.md)|适用于 Teams 客户端的软件更新。|


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkSoftwareUpdateHealth"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkSoftwareUpdateHealth",
  "adminAgentSoftwareUpdateStatus": {
    "@odata.type": "microsoft.graph.teamworkSoftwareUpdateStatus"
  },
  "companyPortalSoftwareUpdateStatus": {
    "@odata.type": "microsoft.graph.teamworkSoftwareUpdateStatus"
  },
  "firmwareSoftwareUpdateStatus": {
    "@odata.type": "microsoft.graph.teamworkSoftwareUpdateStatus"
  },
  "operatingSystemSoftwareUpdateStatus": {
    "@odata.type": "microsoft.graph.teamworkSoftwareUpdateStatus"
  },
  "partnerAgentSoftwareUpdateStatus": {
    "@odata.type": "microsoft.graph.teamworkSoftwareUpdateStatus"
  },
  "teamsClientSoftwareUpdateStatus": {
    "@odata.type": "microsoft.graph.teamworkSoftwareUpdateStatus"
  }
}
```

