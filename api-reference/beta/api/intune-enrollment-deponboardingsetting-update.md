---
title: 更新 depOnboardingSetting
description: 更新 depOnboardingSetting 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ab48db3a056cc02a3631fff9755e27883001d871d6e9f7d2ba703cb54c549242
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54213996"
---
# <a name="update-deponboardingsetting"></a>更新 depOnboardingSetting

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [depOnboardingSetting 对象](../resources/intune-enrollment-deponboardingsetting.md) 的属性。

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
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) 对象的 JSON 表示形式。

下表显示创建 [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 UUID|
|appleIdentifier|String|用于获取当前令牌的 Apple ID。|
|tokenExpirationDateTime|DateTimeOffset|令牌将过期的时间。|
|lastModifiedDateTime|DateTimeOffset|载入服务时。|
|lastSuccessfulSyncDateTime|DateTimeOffset|服务最后一次与 Intune 进行联合时|
|lastSyncTriggeredDateTime|DateTimeOffset|Intune 上次请求同步时。|
|shareTokenWithSchoolDataSyncService|布尔值|是否使用服务启用 Dep 令牌学校数据同步共享。|
|lastSyncErrorCode|Int32|Apple 在上次取消同步期间报告的错误代码。|
|tokenType|[depTokenType](../resources/intune-enrollment-deptokentype.md)|获取或设置 Dep 令牌类型。 可取值为：`none`、`dep`、`appleSchoolManager`。|
|tokenName|字符串|Dep 令牌的友好名称|
|syncedDeviceCount|Int32|获取同步的设备计数|
|dataSharingConsentGranted|布尔值|同意与 Apple Dep 服务共享数据|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
Content-type: application/json
Content-length: 576

{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "appleIdentifier": "Apple Identifier value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
  "lastSyncTriggeredDateTime": "2017-01-01T00:00:02.0916369-08:00",
  "shareTokenWithSchoolDataSyncService": true,
  "lastSyncErrorCode": 1,
  "tokenType": "dep",
  "tokenName": "Token Name value",
  "syncedDeviceCount": 1,
  "dataSharingConsentGranted": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 689

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
  "dataSharingConsentGranted": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




