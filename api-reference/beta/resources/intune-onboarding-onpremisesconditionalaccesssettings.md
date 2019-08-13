---
title: onPremisesConditionalAccessSettings 资源类型
description: 表示租户的 Exchange 本地条件访问设置的单例实体。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c2a696696a25382778ef043d6dcae1320ed75a58
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358011"
---
# <a name="onpremisesconditionalaccesssettings-resource-type"></a>onPremisesConditionalAccessSettings 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示租户的 Exchange 本地条件访问设置的单例实体。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 onPremisesConditionalAccessSettings](../api/intune-onboarding-onpremisesconditionalaccesssettings-get.md)|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|读取 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 对象的属性和关系。|
|[更新 onPremisesConditionalAccessSettings](../api/intune-onboarding-onpremisesconditionalaccesssettings-update.md)|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|更新 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|尚未记录|
|enabled|布尔值|指示是否为该组织启用了本地条件访问|
|includedGroups|Guid 集合|本地条件访问将面向的用户组。 这些组中的所有用户都需要托管移动设备并符合邮件访问的要求。|
|excludedGroups|Guid 集合|将由本地条件访问豁免的用户组。 这些组中的所有用户都将从条件访问策略中豁免。|
|overrideDefaultRule|Boolean|允许设备时重写默认访问规则以确保授予访问。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onPremisesConditionalAccessSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "String (identifier)",
  "enabled": true,
  "includedGroups": [
    "Guid"
  ],
  "excludedGroups": [
    "Guid"
  ],
  "overrideDefaultRule": true
}
```



