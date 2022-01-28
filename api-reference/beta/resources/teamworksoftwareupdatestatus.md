---
title: teamworkSoftwareUpdateStatus 资源类型
description: 表示有关启用了 Microsoft Teams 的设备中各种组件（如管理员代理、公司门户、固件、操作系统、合作伙伴代理和 Microsoft Teams 客户端）的软件更新状态的详细信息。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a50046c758db26ae1d53507263c65dba7aff7435
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262342"
---
# <a name="teamworksoftwareupdatestatus-resource-type"></a>teamworkSoftwareUpdateStatus 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关各种组件（如启用了 Microsoft Teams 的设备中的管理员代理、公司门户、固件、操作系统、合作伙伴代理和 Microsoft Teams 客户端）的软件更新状态的详细信息。[](../resources/teamworkdevice.md) 它指示是否需要软件更新。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|availableVersion|String|要更新的可用软件版本。|
|currentVersion|String|当前软件版本。|
|softwareFreshness|teamworkSoftwareFreshness|软件的更新状态。 可能的值包括 `unknown`、`latest`、`updateAvailable`、`unknownFutureValue`。|


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkSoftwareUpdateStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkSoftwareUpdateStatus",
  "availableVersion": "String",
  "currentVersion": "String",
  "softwareFreshness": "String"
}
```

