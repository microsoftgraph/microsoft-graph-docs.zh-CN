---
title: hybridAgentUpdaterConfiguration 资源类型
description: hybridAgentUpdaterConfiguration 资源类型。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: c81d48053e7fb26eaee678da4e4b33708717e3c1
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722396"
---
# <a name="hybridagentupdaterconfiguration-resource-type"></a>hybridAgentUpdaterConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

租户管理员可以为每个 onPremisesPublishingProfile 配置一个时间窗口，在此时段内，代理可以接收对代理的更新或延迟更新。 为 onPremisesPublishingProfile 指定的 hybridAgentUpdaterConfiguration 适用于该 onPremisesPublishingProfile 内的所有代理。

例如，对于 onPremisesPublishingProfile 类型为"provisioning"的代理，步骤可能如下所示。

1) 租户管理员可以配置为在接下来 n 天内不接收预配代理的任何更新。
2) 租户管理员可以配置更新窗口 (和结束) 代理可以接收更新的时间。
3) 租户管理员可以启用 allowUpdateConfigurationOverride，这将覆盖预配代理的更新程序配置，并禁止他们接收下一个可用更新。

更新程序配置中指定的 DateTime/Time 信息将转换为代理在升级期间报告的本地时区。

代理的更新将遵循以下优先级列表

1) 如果 allowUpdateConfigurationOverride 设置为 true，将跳过租户设置的更新程序配置，当代理的下一个版本可用时，代理将收到更新 (优先级为 1) 。
2) 如果设置了延迟更新，则直到延迟更新日期时间设置为优先级为 2 时 (代理) 。
3) 如果设置更新窗口，则仅在该时间窗口的 24 小时内更新代理 (优先级为 3) 。
4) 如果租户未设置有效的更新程序配置，代理将在代理的下一版本可用时收到更新

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|allowUpdateConfigurationOverride|布尔|指示是否跳过更新程序配置，当代理的下一个版本可用时，代理将收到更新。|
|deferUpdateDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
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


