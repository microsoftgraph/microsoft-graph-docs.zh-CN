---
title: 更新 vppToken
description: 更新 vppToken 对象的属性。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3f57923cee1a6dd261a45d1c31bc3d4ec58e4c59
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59026355"
---
# <a name="update-vpptoken"></a>更新 vppToken

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementServiceConfig.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的 JSON 表示形式。

下表显示创建 [vppToken](../resources/intune-onboarding-vpptoken.md) 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|这是创建 appleVolumePurchaseProgramToken 时自动生成的。 它是实体的键。|
|organizationName|String|与 Apple Volume Purchase Program 令牌关联的组织|
|vppTokenAccountType|[vppTokenAccountType](../resources/intune-shared-vpptokenaccounttype.md)|与给定的 Apple Volume Purchase Program 令牌关联的批量购买计划的类型。 可取值为：`business`、`education`。 可取值为：`business`、`education`。|
|appleId|String|与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。|
|expirationDateTime|DateTimeOffset|Apple Volume Purchase Program 令牌的到期日期时间。|
|lastSyncDateTime|DateTimeOffset|上次利用 Apple Volume Purchase Program 服务并使用 Apple Volume Purchase Program 令牌完成应用程序同步的时间。|
|token|String|从 Apple Volume Purchase Program 下载的 Apple Volume Purchase Program 令牌字符串。|
|lastModifiedDateTime|DateTimeOffset|与 Apple Volume Purchase Program 令牌关联的上次修改日期时间。|
|state|[vppTokenState](../resources/intune-onboarding-vpptokenstate.md)|Apple Volume Purchase Program 令牌的当前状态。 可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。 可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。|
|lastSyncStatus|[vppTokenSyncStatus](../resources/intune-onboarding-vpptokensyncstatus.md)|使用 Apple Volume Purchase Program 令牌触发的上一次应用程序同步的当前同步状态。 可取值为：`none`、`inProgress`、`completed`、`failed`。 可取值为：`none`、`inProgress`、`completed`、`failed`。|
|automaticallyUpdateApps|Boolean|是否自动更新适用于 VPP 令牌的应用。|
|countryOrRegion|String|是否自动更新适用于 VPP 令牌的应用。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}
Content-type: application/json
Content-length: 461

{
  "@odata.type": "#microsoft.graph.vppToken",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "state": "valid",
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 574

{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "9ceb2f92-2f92-9ceb-922f-eb9c922feb9c",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "valid",
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value"
}
```




