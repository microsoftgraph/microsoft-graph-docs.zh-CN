---
title: 更新 depOnboardingSetting
description: 更新 depOnboardingSetting 对象的属性。
ms.openlocfilehash: 931df96b837610044a8c9337fa1fbd5de2a3d52d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041540"
---
# <a name="update-deponboardingsetting"></a>更新 depOnboardingSetting

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

更新[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)对象的属性。
## <a name="prerequisites"></a>先决条件
需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。


|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementServiceConfig.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|Accept|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)对象的 JSON 表示形式。

下表显示时创建[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 UUID|
|appleIdentifier|String|Apple ID 用来获取当前的令牌。|
|tokenExpirationDateTime|DateTimeOffset|该令牌将过期时。|
|lastModifiedDateTime|DateTimeOffset|当该服务已 onboarded。|
|lastSuccessfulSyncDateTime|DateTimeOffset|当服务与 Intune 的最后一个 syned|
|lastSyncTriggeredDateTime|DateTimeOffset|当 Intune 上次请求同步。|
|shareTokenWithSchoolDataSyncService|布尔|是否 Dep 令牌共享将启用学校数据同步服务。|
|lastSyncErrorCode|Int32|在最后一个 dep 同步过程中由 Apple 报告的错误代码。|
|tokenType|[depTokenType](../resources/intune-enrollment-deptokentype.md)|获取或设置 Dep 标记类型。 可取值为：`none`、`dep`、`appleSchoolManager`。|
|tokenName|字符串|Dep 令牌的友好名称|
|syncedDeviceCount|Int32|获取同步设备计数|
|defaultProfileDisplayName|字符串|获取同步设备计数|
|dataSharingConsentGranted|布尔|授予许可与 Apple Dep 服务共享的数据|



## <a name="response"></a>响应
如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)对象。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
Content-type: application/json
Content-length: 589

{
  "appleIdentifier": "Apple Identifier value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
  "lastSyncTriggeredDateTime": "2017-01-01T00:00:02.0916369-08:00",
  "shareTokenWithSchoolDataSyncService": true,
  "lastSyncErrorCode": 1,
  "tokenType": "dep",
  "tokenName": "Token Name value",
  "syncedDeviceCount": 1,
  "defaultProfileDisplayName": "Default Profile Display Name value",
  "dataSharingConsentGranted": true
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 697

{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "id": "40342229-2229-4034-2922-344029223440",
  "appleIdentifier": "Apple Identifier value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
  "lastSyncTriggeredDateTime": "2017-01-01T00:00:02.0916369-08:00",
  "shareTokenWithSchoolDataSyncService": true,
  "lastSyncErrorCode": 1,
  "tokenType": "dep",
  "tokenName": "Token Name value",
  "syncedDeviceCount": 1,
  "defaultProfileDisplayName": "Default Profile Display Name value",
  "dataSharingConsentGranted": true
}
```





