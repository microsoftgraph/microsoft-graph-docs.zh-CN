---
title: linkedResource 资源类型
description: 表示 todoTask 的源
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0a386cd8ed714a6f7127ea0a872a4170997bb8b9
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849905"
---
# <a name="linkedresource-resource-type"></a>linkedResource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示合作伙伴应用程序中与 [todoTask 相关的项目](./todotask.md)。 例如，创建了任务的电子邮件。 **linkedResource**对象存储有关该源应用程序的信息，并允许您链接回相关项。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 linkedResources](../api/todotask-list-linkedresources.md)|[linkedResource](../resources/linkedresource.md) 集合|从 linkedResources 导航属性中获取 linkedResources。|
|[创建 linkedResource](../api/todotask-post-linkedresources.md)|[linkedResource](../resources/linkedresource.md)|创建新的 linkedResources 对象。|
|[获取 linkedResource](../api/linkedresource-get.md)|[linkedResource](../resources/linkedresource.md)|读取 [linkedResource 对象的属性和](../resources/linkedresource.md) 关系。|
|[更新 linkedResource](../api/linkedresource-update.md)|[linkedResource](../resources/linkedresource.md)|更新 [linkedResource 对象的](../resources/linkedresource.md) 属性。|
|[删除 linkedResource](../api/linkedresource-delete.md)|无|删除 [linkedResource](../resources/linkedresource.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|applicationName|String|指示发送 linkedResource 的源的应用 **名称的字段**。|
|displayName|String|指示 **linkedResource 标题的域**。|
|externalId|String|与第三方/合作伙伴系统上的此任务相关联的对象的 ID。|
|id|String|**linkedResource 的服务器生成的**ID。 继承自 [实体](../resources/entity.md)。|
|webUrl|String|到 **linkedResource 的深度链接**。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.linkedResource",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.linkedResource",
  "id": "String (identifier)",
  "webUrl": "String",
  "applicationName": "String",
  "displayName": "String",
  "externalId": "String"
}
```

