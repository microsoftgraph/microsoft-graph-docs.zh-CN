---
title: linkedResource 资源类型
description: 表示 todoTask 的源。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 102b7a918d7f6dbd76db42b738a741b9797aeafb
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313483"
---
# <a name="linkedresource-resource-type"></a>linkedResource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示与 [todoTask](./todotask.md)相关的合作伙伴应用程序中的项。 例如，创建任务的位置的电子邮件。 **LinkedResource**对象存储有关该源应用程序的信息，并允许您链接回相关项目。 您可以在任务详细信息视图中查看 **linkedResource** ，如下所示。

![任务详细信息窗格中的链接资源](/graph/images/todo-linkedresource-taskdetail.png)

有些 **linkedResource** 对象不与任何 web url 相关联，在这种情况下，不需要 **webUrl** 属性。 例如，链接的项可以来自自定义的业务应用程序或本机平台应用程序，例如移动电话上的 SMS 应用程序。 以下是 **linkedResource** 的显示方式和不带 URL 的显示方式。

![具有和不具有 URL 的链接的资源](/graph/images/todo-linkedresource.png)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 linkedResources](../api/todotask-list-linkedresources.md)|[linkedResource](../resources/linkedresource.md) 集合|从 linkedResources 导航属性中获取 linkedResources。|
|[创建 linkedResource](../api/todotask-post-linkedresources.md)|[linkedResource](../resources/linkedresource.md)|创建新的 linkedResources 对象。|
|[获取 linkedResource](../api/linkedresource-get.md)|[linkedResource](../resources/linkedresource.md)|读取 [linkedResource](../resources/linkedresource.md) 对象的属性和关系。|
|[更新 linkedResource](../api/linkedresource-update.md)|[linkedResource](../resources/linkedresource.md)|更新 [linkedResource](../resources/linkedresource.md) 对象的属性。|
|[删除 linkedResource](../api/linkedresource-delete.md)|无|删除一个 [linkedResource](../resources/linkedresource.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|applicationName|String|指示发送 **linkedResource**的源的应用程序名称的字段。|
|displayName|字符串|指示 **linkedResource**的标题的字段。|
|externalId|String|与第三方/合作伙伴系统上的此任务相关联的对象的 Id。|
|id|字符串|服务器为 **linkedResource**生成的 ID。 继承自 [entity](../resources/entity.md)。|
|webUrl|String|指向 **linkedResource**的深层链接。|

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



