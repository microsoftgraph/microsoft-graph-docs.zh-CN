---
title: linkedResource_v2资源类型
description: 表示合作伙伴应用程序中与 baseTask 相关的项
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 720fd4e10664f4f83a0c050d6b4838d68e3f59c7
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820997"
---
# <a name="linkedresource_v2-resource-type-deprecated"></a>linkedResource_v2资源类型 (已弃用) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [todo-deprecate-basetaskapi](../includes/todo-deprecate-basetaskapi.md)]

表示合作伙伴应用程序中与 [baseTask](./basetask.md) 相关的项。 一个示例是创建任务时的电子邮件。 **linkedResource** 对象存储有关该源应用程序的信息，并允许链接回相关项。 可以在任务详细信息视图中看到 **linkedResource** ，如下所示。

![显示任务详细信息窗格中的链接资源卡的屏幕截图。 链接资源卡片显示“在 Jira 中打开”（即合作伙伴应用程序名称）和社交媒体计划（即链接资源的标题）](/graph/images/todo-linkedresource-taskdetail.png)

某些 **linkedResource** 对象不与任何 Web URL 相关联，在这种情况下，不需要 **webUrl** 属性。 例如，链接项可以来自自定义商业应用或本机平台应用，例如移动电话上的短信应用。 下面是 **linkedResource** 与 URL 以及不带 URL 的显示方式。

![显示如何显示带 URL 和不带 URL 的链接资源卡的图像。 带 URL 的链接资源卡包含“使用合作伙伴应用程序名称打开”，而没有 URL 的链接资源卡只包含合作伙伴应用程序名称。](/graph/images/todo-linkedresource.png)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出linkedResource_v2](../api/basetask-list-linkedresources.md)|[linkedResource_v2](../resources/linkedresource_v2.md) 集合|获取 [linkedResource_v2](../resources/linkedresource_v2.md) 对象及其属性的列表。|
|[创建linkedResource_v2](../api/basetask-post-linkedresources.md)|[linkedResource_v2](../resources/linkedresource_v2.md)|创建新的 [linkedResource_v2](../resources/linkedresource_v2.md) 对象。|
|[获取linkedResource_v2](../api/linkedresource_v2-get.md)|[linkedResource_v2](../resources/linkedresource_v2.md)|读取 [linkedResource_v2](../resources/linkedresource_v2.md) 对象的属性和关系。|
|[更新linkedResource_v2](../api/linkedresource_v2-update.md)|[linkedResource_v2](../resources/linkedresource_v2.md)|更新 [linkedResource_v2](../resources/linkedresource_v2.md) 对象的属性。|
|[删除linkedResource_v2](../api/linkedresource_v2-delete.md)|无|删除 [linkedResource_v2](../resources/linkedresource_v2.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|applicationName|String|指示发送 **linkedResource** 的源的应用名称的字段。|
|displayName|String|指示 **linkedResource** 的标题的字段。|
|externalId|String|与第三方/合作伙伴系统上的此任务关联的对象的 ID。|
|id|String|**链接资源** 的服务器生成的 ID。 继承自 [entity](../resources/entity.md)。|
|webUrl|String|**指向 linkedResource** 的深层链接。|

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

