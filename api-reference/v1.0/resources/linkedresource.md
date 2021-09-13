---
title: linkedResource 资源类型
description: 表示 todoTask 的源
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: dfc5e05403c93f07f48c010b8d7233543021f52c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036149"
---
# <a name="linkedresource-resource-type"></a>linkedResource 资源类型

命名空间：microsoft.graph


表示合作伙伴应用程序中与 [todoTask 相关的项目](./todotask.md)。 例如，创建任务时收到的电子邮件。 **linkedResource** 对象存储有关该源应用程序的信息，并允许您链接回相关项。 可以在任务 **详细信息视图中看到 linkedResource，** 如下所示。

![任务详细信息窗格中的链接资源](/graph/images/todo-linkedresource-taskdetail.png)

某些 **linkedResource** 对象不与任何 Web URL 关联，在这种情况下，不需要 **webUrl** 属性。 例如，链接项可以来自自定义业务应用或本机平台应用，如手机上的短信应用。 下面是 **linkedResource 如何** 显示（带和不带 URL）。

![具有或不带 URL 的链接资源](/graph/images/todo-linkedresource.png)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 linkedResources](../api/todotask-list-linkedresources.md)|[linkedResource](../resources/linkedresource.md) 集合|从 linkedResources 导航属性获取 linkedResources。|
|[创建 linkedResource](../api/todotask-post-linkedresources.md)|[linkedResource](../resources/linkedresource.md)|创建新的 linkedResources 对象。|
|[获取 linkedResource](../api/linkedresource-get.md)|[linkedResource](../resources/linkedresource.md)|读取 [linkedResource](../resources/linkedresource.md) 对象的属性和关系。|
|[更新 linkedResource](../api/linkedresource-update.md)|[linkedResource](../resources/linkedresource.md)|更新 [linkedResource 对象](../resources/linkedresource.md) 的属性。|
|[删除 linkedResource](../api/linkedresource-delete.md)|None|删除 [linkedResource](../resources/linkedresource.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|applicationName|String|指示发送 **linkedResource** 的源的应用名称的字段。|
|displayName|String|指示 **linkedResource 的标题的字段**。|
|externalId|String|第三方/合作伙伴系统上与此任务关联的对象的 ID。|
|id|String|服务器为 **linkedResource** 生成的 ID。 继承自 [实体](../resources/entity.md)。|
|WebUrl|String|指向 **linkedResource 的深层链接**。|

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



