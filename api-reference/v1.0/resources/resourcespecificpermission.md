---
title: resourceSpecificPermission 资源类型
description: 表示用于授权应用程序直接访问特定资源实例数据的权限
author: psignoret
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: bc1cd89ba26629b59c83fdd6b626cb280f69eaab
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63376384"
---
# <a name="resourcespecificpermission-resource-type"></a>resourceSpecificPermission 资源类型

命名空间：microsoft.graph

表示用于授权应用程序直接访问特定资源实例（如聊天或团队）的数据的权限。 例如，特定于资源的权限 ChannelMessage.Read.Group 允许Microsoft Teams读取单个团队的频道消息。 

只有使用 Microsoft Teams API 访问特定聊天和团队Graph特定权限。 有关详细信息，请参阅资源[特定的应用程序Teams许可](/microsoftteams/platform/graph-api/rsc/resource-specific-consent)。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|说明|String|描述特定于资源的权限表示的访问级别。|
|displayName|String|资源显示名称权限的组。|
|id|Guid|特定于资源的应用程序权限的唯一标识符。|
|isEnabled|Boolean|指示是否启用权限。|
|value|String|权限的值。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceSpecificPermission"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceSpecificPermission",
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isEnabled": "Boolean",
  "value": "String"
}
```
