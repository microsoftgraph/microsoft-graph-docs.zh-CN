---
title: serviceUpdateMessageViewpoint 资源类型
description: 表示 serviceUpdateMessage 的用户视图点数据。"
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 080d739d2111d383c5e5d7cf8ec3ec510e1cb5ba
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59108763"
---
# <a name="serviceupdatemessageviewpoint-resource-type"></a>serviceUpdateMessageViewpoint 资源类型

命名空间：microsoft.graph

表示 [serviceUpdateMessage](../resources/serviceupdatemessage.md)的用户视图点数据。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|isArchived|Boolean|指示用户是否已存档邮件。|
|isFavorited|Boolean|指示用户是否将邮件标记为收藏夹。|
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
