---
title: hybridAgentUpdaterConfiguration 资源类型
description: hybridAgentUpdaterConfiguration 资源类型。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5c3efdd55f432add28f6d13797a0f73b4458b966
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841246"
---
# <a name="hybridagentupdaterconfiguration-resource-type"></a>hybridAgentUpdaterConfiguration 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

租户管理员可以为每个 onPremisesPublishingProfile 配置一个时间段, 在此时段内, 代理可以接收更新或将更新推迟到代理。 为 onPremisesPublishingProfile 指定的 hybridAgentUpdaterConfiguration 适用于该 onPremisesPublishingProfile 中的所有代理。

例如, 对于 onPremisesPublishingProfile 中类型为 "预配" 的代理, 这些步骤可能如下所示。

1) 租户管理员可以配置为在接下来的 n 天中不接收对预配代理的任何更新。
2) 租户管理员可以配置更新窗口 (开始和结束时间), 在此期间, 代理可以 recive 更新。
3) 租户管理员可以启用 allowUpdateConfigurationOverride, 这将覆盖预配代理的更新 configutration, 并 alows 他们接收下一个可用的更新。

在更新配置过程中指定的 DateTime/Time 信息将转换为 evaluvation 期间代理报告的本地时区。

代理的更新将遵循以下优先级列表

1) 如果将 allowUpdateConfigurationOverride 设置为 true, 则将跳过租户设置的更新配置, 并且代理将在下一版本的代理可用时收到更新 (优先级为 1)。
2) 如果设置了延迟更新, 将不会更新代理, 直到延迟更新日期时间 (优先级 2)。
3) 如果设置了 "更新" 窗口, 则代理将仅在24小时内 (优先级为 3) 的该时间段内更新。
4) 如果租户未设置有效的更新程序配置, 则代理将在下一版本的代理可用时收到更新。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|allowUpdateConfigurationOverride|Boolean|指示是否将跳过更新配置, 并且代理将在下一版本的代理可用时收到更新。|
|deferUpdateDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|updateWindow|[updateWindow](updatewindow.md)||

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.hybridAgentUpdaterConfiguration",
  "baseType": null
}-->

```json
{
  "allowUpdateConfigurationOverride": true,
  "deferUpdateDateTime": "String (timestamp)",
  "updateWindow": {"@odata.type": "microsoft.graph.updateWindow"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "hybridAgentUpdaterConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
