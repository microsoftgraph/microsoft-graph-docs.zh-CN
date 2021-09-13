---
title: workforceIntegration 资源类型
description: 员工与班次集成的实例。
ms.localizationpriority: medium
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c9c346852df97abb93014ad417bd1948b19ef975
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134141"
---
# <a name="workforceintegration-resource-type"></a>workforceIntegration 资源类型

命名空间：microsoft.graph

员工与班次集成的实例。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [Create](../api/workforceintegration-post.md) | [workforceIntegration](workforceintegration.md) | 创建新的 **workforceIntegration** 对象。|
| [List](../api/workforceintegration-list.md) | [workforceIntegration](workforceintegration.md) 集合 | 获取与此 **计划关联的 workforceIntegration** 对象列表。|
| [Get](../api/workforceintegration-get.md) | [workforceIntegration](workforceintegration.md) | 读取 **workforceIntegration** 对象的属性和关系。 |
| [更新](../api/workforceintegration-update.md) | [workforceIntegration](workforceintegration.md) | 更新 **一个 workforceIntegration** 对象。 |
| [删除](../api/workforceintegration-delete.md) | 无 | 删除 **一个 workforceIntegration** 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|apiVersion|Int32|用于回叫 URL 的 API 版本。 从 1 开始。|
|displayName|String|员工集成的名称。|
|加密|[workforceIntegrationEncryption](workforceintegrationencryption.md)|员工集成加密资源。|
|isActive|Boolean|指示此员工集成当前是否处于活动状态且可用。|
|supportedEntities|workforceIntegrationSupportedEntities | 同步更改通知支持的 Shifts 实体。 班次将调用此处添加的这些实体上客户端更改时提供的 URL。 默认情况下，更改通知不支持任何实体。 可取值为：`none`、`shift`、`swapRequest`、`userShiftPreferences`、`openshift`、`openShiftRequest`、`offerShiftRequest`、`unknownFutureValue`。|
|url|String| 用于从 Shifts 服务进行回调的员工集成 URL。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workforceIntegration"
}-->

```json
{
  "apiVersion": 1024,
  "displayName": "String",
  "encryption": {"@odata.type": "microsoft.graph.workforceIntegrationEncryption"},
  "isActive": true,
  "supportedEntities": "string",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workforceIntegration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

