---
title: 更新 targetedManagedAppConfigurationPolicySetItem
description: 更新 targetedManagedAppConfigurationPolicySetItem 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a938784fcd089c2deabd70aed2b431dba9b7e876
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266007"
---
# <a name="update-targetedmanagedappconfigurationpolicysetitem"></a>更新 targetedManagedAppConfigurationPolicySetItem

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [targetedManagedAppConfigurationPolicySetItem 对象](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) 的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [targetedManagedAppConfigurationPolicySetItem](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) 对象的 JSON 表示形式。

下表显示创建 [targetedManagedAppConfigurationPolicySetItem 时所需的属性](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|PolicySetItem 的键。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|createdDateTime|DateTimeOffset|PolicySetItem 的创建时间。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|lastModifiedDateTime|DateTimeOffset|PolicySetItem 的上次修改时间。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|payloadId|字符串|PolicySetItem 的 PayloadId。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|itemType|字符串|PolicySetItem 的 policySetType。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|displayName|字符串|PolicySetItem 的 DisplayName。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|status|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|PolicySetItem 的状态。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。 可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|错误代码（如果发生了任何错误）。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。 可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。|
|guidedDeploymentTags|String collection|引导式部署的标记 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [targetedManagedAppConfigurationPolicySetItem](../resources/intune-policyset-targetedmanagedappconfigurationpolicysetitem.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
Content-type: application/json
Content-length: 326

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfigurationPolicySetItem",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ]
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 498

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfigurationPolicySetItem",
  "id": "f86d3112-3112-f86d-1231-6df812316df8",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ]
}
```




