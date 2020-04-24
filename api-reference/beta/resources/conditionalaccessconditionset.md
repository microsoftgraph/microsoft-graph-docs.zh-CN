---
title: conditionalAccessConditionSet 资源类型
description: 表示在应用策略时控制的条件的类型。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f5db4c6367834733a4a5fbbb6c7a8d6b08393160
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805678"
---
# <a name="conditionalaccessconditionset-resource-type"></a>conditionalAccessConditionSet 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在应用策略时控制的条件的类型。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|来说|[conditionalAccessApplications](conditionalaccessapplications.md)| 策略中包含和排除的应用程序和用户操作。 必需。 |
|users|[conditionalAccessUsers](conditionalaccessusers.md)| 策略中包含和排除的用户、组和角色。 必需。 |
|clientAppTypes|String 集合| 策略中包含的客户端应用程序类型。 可取值为：`browser`、`modern`、`easSupported`、`easUnsupported`、`other`。|
|deviceStates|[conditionalAccessDeviceStates](conditionalaccessdevicestates.md)| 策略中的设备状态。 |
|驱动器|[conditionalAccessDevices](conditionalaccessdevices.md)| 策略中的设备。 |
|位置|[conditionalAccessLocations](conditionalaccesslocations.md)| 策略中包含和排除的位置。 |
|平台|[conditionalAccessPlatforms](conditionalaccessplatforms.md)| 策略中包含和排除的平台。 |
|signInRiskLevels|String 集合| 策略中包括的风险级别。 可取值为：`low`、`medium`、`high`、`none`。|

>**注意：** 我们正在弃用**deviceStates**条件，将来可能会将其删除。 接下来，使用 "**设备**" 条件。

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "clientAppTypes",
    "deviceStates",
    "devices",
    "locations",
    "platforms",
    "signInRiskLevels"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessConditionSet",
  "baseType": null
}-->

```json
{
  "applications": {"@odata.type": "microsoft.graph.conditionalAccessApplications"},
  "users": {"@odata.type": "microsoft.graph.conditionalAccessUsers"},
  "clientAppTypes": ["String"],
  "deviceStates": {"@odata.type": "microsoft.graph.conditionalAccessDeviceStates"},
  "devices": {"@odata.type": "microsoft.graph.conditionalAccessDevices"},
  "locations": {"@odata.type": "microsoft.graph.conditionalAccessLocations"},
  "platforms": {"@odata.type": "microsoft.graph.conditionalAccessPlatforms"},
  "signInRiskLevels": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessConditionset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
