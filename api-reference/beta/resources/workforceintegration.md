---
title: workforceIntegration 资源类型
description: 员工的一个实例与倒班的集成。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1e836a4346fe5e31f39c1f6383acbf78530ae9e6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519083"
---
# <a name="workforceintegration-resource-type"></a>workforceIntegration 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

员工的一个实例与倒班的集成。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取](../api/workforceintegration-get.md) | [workforceIntegration](workforceintegration.md) | 读取**workforceIntegration**对象的属性和关系。 |
| [更新](../api/workforceintegration-update.md) | [workforceIntegration](workforceintegration.md) | 更新**workforceIntegration**对象。 |
| [删除](../api/workforceintegration-delete.md) | 无 | 删除**workforceIntegration**对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|apiVersion|Int32|回调 URL 的 API 版本。 从1开始。|
|displayName|String|劳动力集成的名称。|
|技术|[workforceIntegrationEncryption](workforceintegrationencryption.md)|劳动力集成加密资源。|
|isActive|布尔|指示此劳动力集成当前是否处于活动状态且可用。|
|支持|string| 可能的值为`none`： `shift`、 `swapRequest`、 `openshift` `openShiftRequest`、、`userShiftPreferences`|
|url|String| 劳动力集成 URL，用于从班次服务进行回调。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workforceIntegration",
  "baseType": ""
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
