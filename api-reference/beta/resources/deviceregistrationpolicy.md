---
title: deviceRegistrationPolicy 资源类型
description: 表示控制 Azure Active Directory 租户的配额限制、其他身份验证和授权策略的策略范围。
author: myra-ramdenbourg
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: f810529cffc5c5c5c5a19d3fa2644aba5874d53e
ms.sourcegitcommit: c168f2cb95b4863080a84cc199a7b878fb5eeb8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2022
ms.locfileid: "66690076"
---
# <a name="deviceregistrationpolicy-resource-type"></a>deviceRegistrationPolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示控制配额限制、其他身份验证和授权策略以向组织注册设备标识的策略范围。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[获取 deviceRegistrationPolicy](../api/deviceregistrationpolicy-get.md)|[deviceRegistrationPolicy](../resources/deviceregistrationpolicy.md)|读取 [deviceRegistrationPolicy 对象的](../resources/deviceregistrationpolicy.md) 属性。|
|[更新 deviceRegistrationPolicy](../api/deviceregistrationpolicy-update.md)|[deviceRegistrationPolicy](../resources/deviceregistrationpolicy.md)|更新 [deviceRegistrationPolicy 对象的](../resources/deviceregistrationpolicy.md) 属性。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|azureADJoin|[azureAdJoinPolicy](../resources/azureadjoinpolicy.md)|指定用于在组织内使用 **Azure AD Join** 控制新设备注册的授权策略。 必填。 有关详细信息，请参阅[什么是设备标识？](/azure/active-directory/devices/overview)|
|azureADRegistration|[azureADRegistrationPolicy](../resources/azureadregistrationpolicy.md)|指定使用在组织中 **注册的 Azure AD** 控制新设备注册的授权策略。 必填。 有关详细信息，请参阅[什么是设备标识？](/azure/active-directory/devices/overview)|
|说明|字符串|设备注册策略的说明。 它始终设置为 `Tenant-wide policy that manages intial provisioning controls using quota restrictions, additional authentication and authorization checks`。 只读。|
|displayName|String|设备注册策略的名称。 它始终设置为 `Device Registration Policy`。 只读。|
|id|String| 设备注册策略的标识符。 它始终设置为 `deviceRegistrationPolicy`。 只读。|
|multiFactorAuthConfiguration|multiFactorAuthConfiguration|指定用户使用组织内注册的 **Azure AD Join** 或 **Azure AD** 完成注册的身份验证策略。 可能的值包括： `0` (含义 `notRequired`) 、 `1` (含义 `required`) 和 `2` (含义 `unknownFutureValue`) 。 默认值为 `0`。 |
|userDeviceQuota|Int32|指定在阻止新设备注册之前，用户可在组织中拥有的最大设备数。 默认值设置为 50。 如果在策略更新操作期间未指定此属性，则会自动重置 `0` 该属性以指示不允许用户加入任何设备。 |


## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceRegistrationPolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceRegistrationPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "userDeviceQuota": "Integer",
  "multiFactorAuthConfiguration": "String",
  "azureADRegistration": {
    "@odata.type": "microsoft.graph.azureADRegistrationPolicy"
  },
  "azureADJoin": {
    "@odata.type": "microsoft.graph.azureAdJoinPolicy"
  }
}
```
