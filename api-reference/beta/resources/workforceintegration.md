---
title: workforceIntegration 资源类型
description: 员工与班次集成的实例。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 12aa4a6ac8fd72f20a0019a95eeb20196b1ed3bf
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787651"
---
# <a name="workforceintegration-resource-type"></a>workforceIntegration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

员工与班次集成的实例。

## <a name="methods"></a>方法

| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
| [List](../api/workforceintegration-list.md) | [workforceIntegration](workforceintegration.md) 集合 | 获取与此 **计划关联的 workforceIntegration** 对象列表。|
| [创建](../api/workforceintegration-post.md) | [workforceIntegration](workforceintegration.md) | 创建新的 **workforceIntegration** 对象。|
| [获取](../api/workforceintegration-get.md) | [workforceIntegration](workforceintegration.md) | 读取 **workforceIntegration** 对象的属性和关系。 |
| [更新](../api/workforceintegration-update.md) | [workforceIntegration](workforceintegration.md) | 更新 **一个 workforceIntegration** 对象。 |
| [删除](../api/workforceintegration-delete.md) | 无 | 删除 **一个 workforceIntegration** 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|apiVersion|Int32|用于回叫 URL 的 API 版本。 从 1 开始。|
|displayName|String|员工集成的名称。|
|加密|[workforceIntegrationEncryption](workforceintegrationencryption.md)|员工集成加密资源。|
|isActive|Boolean|指示此员工集成当前是否处于活动状态且可用。|
|支持|string| 同步更改通知支持的 Shifts 实体。 班次将调用此处添加的这些实体上客户端更改时提供的 URL。 默认情况下，更改通知不支持任何实体。 可能的值为 `none` `shift` `swapRequest` `openshift` `openShiftRequest` `userShiftPreferences` 、、、、、、、 `offerShiftRequest` `timeCard` `timeOffReason` 和 `timeOff` `timeOffRequest` `unknownFutureValue` 。 如果选择多个值，则所有值必须以大写字母开头。|
|supportedEntities|string| 此属性 **将替换** v1.0 中的 supports。 我们建议你使用此属性，而不是 **支持**。 **目前，supports** 属性在 beta 版中仍受支持。 可能的值为 `none` `shift` `swapRequest` `openshift` `openShiftRequest` `userShiftPreferences` 、、、、、、、 `offerShiftRequest` `timeCard` `timeOffReason` 和 `timeOff` `timeOffRequest` `unknownFutureValue` 。 如果选择多个值，则所有值必须以大写字母开头。|
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
  "supports": "string",
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


