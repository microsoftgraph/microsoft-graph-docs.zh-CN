---
title: conditionalAccessConditionSet 资源类型
description: 表示策略应用时所控制的条件类型。
ms.localizationpriority: medium
author: davidspooner
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3dbd7a5a1a436709deed0bf342718ea81a282798
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519445"
---
# <a name="conditionalaccessconditionset-resource-type"></a>conditionalAccessConditionSet 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示策略应用时所控制的条件类型。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|应用程序|[conditionalAccessApplications](conditionalaccessapplications.md)| 策略中包含和排除的应用程序和用户操作。 必需。 |
|users|[conditionalAccessUsers](conditionalaccessusers.md)| 策略中包含和排除的用户、组和角色。 用户 **或** **clientApplications** 是必需的。 |
|clientApplications|[conditionalAccessClientApplications](../resources/conditionalaccessclientapplications.md)|客户端应用程序 (服务主体和工作负荷) 包含在策略中以及从策略中排除。 用户 **或** **clientApplications** 是必需的。 |
|clientAppTypes|conditionalAccessClientApp 集合| 策略中包含的客户端应用程序类型。 可取值为：`all`、`browser`、`mobileAppsAndDesktopClients`、`exchangeActiveSync`、`easSupported`、`other`。 必需。|
|deviceStates|[conditionalAccessDeviceStates](conditionalaccessdevicestates.md)| 策略中的设备状态。 |
|设备|[conditionalAccessDevices](conditionalaccessdevices.md)| 策略中的设备。 |
|位置|[conditionalAccessLocations](conditionalaccesslocations.md)| 策略中包含的位置和从策略中排除的位置。 |
|平台|[conditionalAccessPlatforms](conditionalaccessplatforms.md)| 策略中包含和排除的平台。 |
|servicePrincipalRiskLevels|riskLevel 集合| 策略中包含的服务主体风险级别。 可取值为：`low`、`medium`、`high`、`none`、`unknownFutureValue`。|
|signInRiskLevels|riskLevel 集合| 策略中包含的登录风险级别。 可取值为：`low`、`medium`、`high`、`hidden`、`none`、`unknownFutureValue`。 必需。|
|userRiskLevels|riskLevel 集合| 策略中包含的用户风险级别。 可取值为：`low`、`medium`、`high`、`hidden`、`none`、`unknownFutureValue`。 必需。|

>**注意：**
>* **clientAppType** `modern` 将被弃用，并替换为 `mobileAppsAndDesktopClients`。 <br>
>* **clientAppType** `easUnsupported` 将弃用， `exchangeActiveSync` 支持包括 EAS 支持和不受支持的平台。 <br>
>* We are deprecating the **deviceStates** condition， and it may be removed in the future. 今后，使用 **设备** 条件。

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
  "@odata.type": "#microsoft.graph.conditionalAccessConditionSet",
  "applications": {"@odata.type": "microsoft.graph.conditionalAccessApplications"},
  "users": {"@odata.type": "microsoft.graph.conditionalAccessUsers"},
  "clientApplications": {"@odata.type": "microsoft.graph.conditionalAccessClientApplications"},
  "clientAppTypes": ["String"],
  "deviceStates": {"@odata.type": "microsoft.graph.conditionalAccessDeviceStates"},
  "devices": {"@odata.type": "microsoft.graph.conditionalAccessDevices"},
  "locations": {"@odata.type": "microsoft.graph.conditionalAccessLocations"},
  "platforms": {"@odata.type": "microsoft.graph.conditionalAccessPlatforms"},
  "servicePrincipalRiskLevels": ["String"],
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


