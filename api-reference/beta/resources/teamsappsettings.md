---
title: teamsAppSettings 资源类型
description: 表示 Teams 应用设置
author: subray2014
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0a36f6657dc8231450514eb6c60d7d729c0e0818
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645628"
---
# <a name="teamsappsettings-resource-type"></a>teamsAppSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示租户中所有 [Teams 应用](teamsapp.md) 的租户范围设置。

继承自 [entity](../resources/entity.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 teamsAppSettings](../api/teamsappsettings-get.md)|[teamsAppSettings](../resources/teamsappsettings.md)|获取租户中所有 Teams 应用的租户范围设置。|
|[更新 teamsAppSettings](../api/teamsappsettings-update.md)|[teamsAppSettings](../resources/teamsappsettings.md)|更新租户中所有 Teams 应用的租户范围设置。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|isChatResourceSpecificConsentEnabled|布尔值|指示是否已为租户启用特定于资源的聊天/会议许可。 如果为 true，则可以在聊天和会议中安装允许在租户中且需要资源特定权限的 Teams 应用。 如果为 false，则会阻止在聊天或会议中安装需要资源特定权限的任何 Teams 应用。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsAppSettings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsAppSettings",
  "id": "String (identifier)",
  "isChatResourceSpecificConsentEnabled": "Boolean"
}
```

## <a name="see-also"></a>另请参阅

- [特定于资源的同意](/microsoftteams/platform/graph-api/rsc/resource-specific-consent)