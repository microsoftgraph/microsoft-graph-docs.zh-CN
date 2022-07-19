---
title: 管理员资源类型
description: 充当管理员功能容器的实体。
author: angelgolfer-ms
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: ce20f9d9a15acbf5c27402eb018b4bbc5ad85b97
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856321"
---
# <a name="admin-resource-type"></a>管理员资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

充当管理员功能容器的实体。

## <a name="properties"></a>属性
无。

## <a name="relationships"></a>关系
|关系|类型|Description|
|:---|:---|:---|
| reportSettings |[microsoft.graph.adminReportSettings](../resources/adminreportsettings.md)|用于管理报表的管理资源的容器。|
| serviceAnnouncement | [serviceAnnouncement](serviceannouncement.md) | 服务通信资源的容器。 只读。 |
| sharepoint |[microsoft.graph.tenantAdmin.sharepoint](../resources/tenantadmin-sharepoint.md)|用于管理 SharePoint 和 OneDrive 租户级别设置的管理资源的容器。|
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

