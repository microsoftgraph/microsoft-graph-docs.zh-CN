---
title: onPremisesConditionalAccessSettings 资源类型
description: 表示租户的 Exchange 本地条件访问设置的单例实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5175d7487aafb9a7e3480e8f4ca263c298b340e3
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58820202"
---
# <a name="onpremisesconditionalaccesssettings-resource-type"></a>onPremisesConditionalAccessSettings 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示租户的 Exchange 本地条件访问设置的单例实体。

## <a name="methods"></a>方法
|方法|返回类型|Description|
|:---|:---|:---|
|[获取 onPremisesConditionalAccessSettings](../api/intune-onboarding-onpremisesconditionalaccesssettings-get.md)|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|读取 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 对象的属性和关系。|
|[更新 onPremisesConditionalAccessSettings](../api/intune-onboarding-onpremisesconditionalaccesssettings-update.md)|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|更新 [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|尚未记录|
|enabled|Boolean|指示是否为该组织启用了本地条件访问|
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



