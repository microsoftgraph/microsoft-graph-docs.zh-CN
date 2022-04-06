---
title: conditionalAccessConditionSet 资源类型
description: 表示策略应用时所控制的条件类型。
ms.localizationpriority: medium
author: davidspooner
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 6bb96bd08f9ffdd3876ba3836b19878b24fad686
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2022
ms.locfileid: "63672544"
---
# <a name="conditionalaccessconditionset-resource-type"></a>conditionalAccessConditionSet 资源类型

命名空间：microsoft.graph

表示策略应用时所控制的条件类型。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|应用程序|[conditionalAccessApplications](conditionalaccessapplications.md)| 策略中包含和排除的应用程序和用户操作。 必需。 |
|users|[conditionalAccessUsers](conditionalaccessusers.md)| 策略中包含和排除的用户、组和角色。 必需。 |
|clientApplications|[conditionalAccessClientApplications](../resources/conditionalaccessclientapplications.md)|客户端应用程序 (服务主体和工作负荷) 包含在策略中以及从策略中排除。 用户 **或** **clientApplications** 是必需的。 |
|clientAppTypes|conditionalAccessClientApp 集合| 策略中包含的客户端应用程序类型。 可取值为：`all`、`browser`、`mobileAppsAndDesktopClients`、`exchangeActiveSync`、`easSupported`、`other`。 必需。|
|设备|[conditionalAccessDevices](conditionalaccessdevices.md)| 策略中的设备。 |
|位置|[conditionalAccessLocations](conditionalaccesslocations.md)| 策略中包含的位置和从策略中排除的位置。 |
|平台|[conditionalAccessPlatforms](conditionalaccessplatforms.md)| 策略中包含和排除的平台。 |
|signInRiskLevels|riskLevel 集合| 策略中包含的登录风险级别。 可取值为：`low`、`medium`、`high`、`hidden`、`none`、`unknownFutureValue`。 必需。|
|userRiskLevels|riskLevel 集合| 策略中包含的用户风险级别。 可取值为：`low`、`medium`、`high`、`hidden`、`none`、`unknownFutureValue`。 必填。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "clientAppTypes",
    "locations",
    "platforms",
    "signInRiskLevels",
    "userRiskLevels"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessConditionSet",
  "baseType": null
}-->

```json
{
  "applications": {"@odata.type": "microsoft.graph.conditionalAccessApplications"},
  "users": {"@odata.type": "microsoft.graph.conditionalAccessUsers"},
  "clientApplications": {"@odata.type": "microsoft.graph.conditionalAccessClientApplications"},
  "clientAppTypes": ["String"],
  "devices": {"@odata.type": "microsoft.graph.conditionalAccessDevices"},
  "locations": {"@odata.type": "microsoft.graph.conditionalAccessLocations"},
  "platforms": {"@odata.type": "microsoft.graph.conditionalAccessPlatforms"},
  "signInRiskLevels": ["String"],
  "userRiskLevels": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessConditionSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

