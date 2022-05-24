---
title: 管理员资源类型
description: 充当管理员功能容器的实体。
author: angelgolfer-ms
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: ef9b235a175b3304b9354beddc67f59eb3994cf1
ms.sourcegitcommit: 10b45b3e666bf6b438803885128bc2f0fa2fa994
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/24/2022
ms.locfileid: "65653495"
---
# <a name="admin-resource-type"></a>管理员资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

充当管理员功能容器的实体。

## <a name="properties"></a>属性
无。

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
| serviceAnnouncement | [serviceAnnouncement](serviceannouncement.md) | 服务通信资源的容器。 只读。 |
| sharepoint |[microsoft.graph.tenantAdmin.sharepoint](../resources/tenantadmin-sharepoint.md)|管理资源的容器，用于管理SharePoint和OneDrive的租户级别设置。|
| windows |[microsoft.graph.windowsUpdates.windows](../resources/windowsupdates-windows.md)|适用于企业的所有Windows 更新部署服务功能的容器。 只读。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.admin",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.admin"
}
```

