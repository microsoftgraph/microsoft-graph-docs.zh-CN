---
title: serviceUpdateMessageViewpoint 资源类型
description: 表示 serviceUpdateMessage 的用户视图点数据。"
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: c84a07691c2507a9ff74102ac6f4b1675cb382e7
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109092"
---
# <a name="serviceupdatemessageviewpoint-resource-type"></a>serviceUpdateMessageViewpoint 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [serviceUpdateMessage](../resources/serviceupdatemessage.md)的用户视图点数据。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|isArchived|Boolean|指示用户是否已存档邮件。|
|isFavorited|布尔值|指示用户是否将邮件标记为收藏夹。|
|isRead|Boolean|指示用户是否阅读邮件。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.serviceUpdateMessageViewpoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceUpdateMessageViewpoint",
  "isRead": "Boolean",
  "isArchived": "Boolean",
  "isFavorited": "Boolean"
}
```