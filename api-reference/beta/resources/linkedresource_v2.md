---
title: linkedResource_v2资源类型
description: 表示合作伙伴应用程序中与 baseTask 相关的项
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: b3c84cf8c4f08800e22841e6928ef85b1162a2e3
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424850"
---
# <a name="linkedresource_v2-resource-type"></a>linkedResource_v2资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示合作伙伴应用程序中与 [baseTask 相关的项目](./basetask.md)。 例如，创建任务时收到的电子邮件。 **linkedResource** 对象存储有关该源应用程序的信息，并允许您链接回相关项。 可以在任务 **详细信息视图中看到 linkedResource，** 如下所示。

![Screenshot showing linked resource card in task details pane. 链接的资源卡显示"在 Jira 中打开"（这是合作伙伴应用程序名称）和"社交媒体计划"（链接资源的标题）](/graph/images/todo-linkedresource-taskdetail.png)

某些 **linkedResource** 对象不与任何 Web URL 关联，在这种情况下，不需要 **webUrl** 属性。 例如，链接项可以来自自定义业务应用或本机平台应用，如手机上的短信应用。 下面是 **linkedResource 如何** 显示（带和不带 URL）。

![显示带和不带 URL 的链接资源卡片显示方式的图像。 具有 URL 的链接资源卡包含"使用合作伙伴应用程序名称打开"，而不带 URL 的链接资源卡仅包含合作伙伴应用程序名称。](/graph/images/todo-linkedresource.png)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出linkedResource_v2](../api/basetask-list-linkedresources.md)|[linkedResource_v2](../resources/linkedresource_v2.md) 集合|获取对象及其 [linkedResource_v2](../resources/linkedresource_v2.md) 列表。|
|[创建linkedResource_v2](../api/basetask-post-linkedresources.md)|[linkedResource_v2](../resources/linkedresource_v2.md)|创建新的 [linkedResource_v2](../resources/linkedresource_v2.md) 对象。|
|[获取linkedResource_v2](../api/linkedresource_v2-get.md)|[linkedResource_v2](../resources/linkedresource_v2.md)|读取 linkedResource_v2 对象的属性 [和](../resources/linkedresource_v2.md) 关系。|
|[更新linkedResource_v2](../api/linkedresource_v2-update.md)|[linkedResource_v2](../resources/linkedresource_v2.md)|更新 linkedResource_v2 [对象的属性](../resources/linkedresource_v2.md) 。|
|[删除linkedResource_v2](../api/linkedresource_v2-delete.md)|无|删除 [linkedResource_v2对象](../resources/linkedresource_v2.md) 。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|applicationName|String|指示发送 **linkedResource** 的源的应用名称的字段。|
|displayName|字符串|指示 **linkedResource 的标题的字段**。|
|externalId|String|第三方/合作伙伴系统上与此任务关联的对象的 ID。|
|id|字符串|服务器为 **linkedResource** 生成的 ID。 继承自 [实体](../resources/entity.md)。|
|WebUrl|String|指向 **linkedResource 的深层链接**。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.linkedResource_v2",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.linkedResource_v2",
  "webUrl": "String",
  "applicationName": "String",
  "displayName": "String",
  "externalId": "String",
  "id": "String (identifier)"
}
```

