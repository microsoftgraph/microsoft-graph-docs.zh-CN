---
title: serviceAnnouncementAttachment 资源类型
description: 表示与 serviceUpdateMessage 对象关联的附件。
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 7acc5906e0054ccd78097caff0863c651fa97dd3
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/01/2022
ms.locfileid: "62291258"
---
# <a name="serviceannouncementattachment-resource-type"></a>serviceAnnouncementAttachment 资源类型

命名空间：microsoft.graph

表示与 [serviceUpdateMessage 对象关联的](../resources/serviceupdatemessage.md) 附件。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 serviceAnnouncementAttachment](../api/serviceannouncementattachment-get.md)|[serviceAnnouncementAttachment](../resources/serviceannouncementattachment.md)|读取 [serviceAnnouncementAttachment](../resources/serviceannouncementattachment.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|content|流|附件内容。|
|contentType|String|附件的内容类型。|
|id|String|附件 ID。 继承自 [实体](../resources/entity.md)。|
|lastModifiedDateTime|DateTimeOffset|上次修改附件的日期和时间。|
|name|String|附件名称。|
|size|Int32|附件大小，以字节为单位。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceAnnouncementAttachment",
  "baseType": "microsoft.graph.attachment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceAnnouncementAttachment",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "name": "String",
  "contentType": "String",
  "size": "Integer",
  "isInline": "Boolean",
  "content": "Stream"
}
```
