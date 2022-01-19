---
title: serviceAnnouncementAttachment 资源类型
description: 表示与 serviceUpdateMessage 对象关联的附件。
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 8b00cacb19784f34700089d59de22183b8f6e98a
ms.sourcegitcommit: bfd1ab7e015ef04cb2ca3fb85d308ba2ce830a89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/19/2022
ms.locfileid: "62072736"
---
# <a name="serviceannouncementattachment-resource-type"></a>serviceAnnouncementAttachment 资源类型

命名空间：microsoft.graph

表示与 [serviceUpdateMessage](../resources/serviceupdatemessage.md) 对象关联的附件。

继承自 [附件](../resources/attachment.md)。

## <a name="methods"></a>Methods
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
