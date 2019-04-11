---
title: 更新 depEnrollmentProfile
description: 更新 depEnrollmentProfile 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 40384682136c84ac957ee39bec3a2b2144e7a6a0
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31787251"
---
# <a name="update-depenrollmentprofile"></a>更新 depEnrollmentProfile

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

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
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中, 提供[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象的 JSON 表示形式。

下表显示创建[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的对象的 GUID|
|displayName|String|继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的配置文件的名称|
|description|String|从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的配置文件的说明|
|requiresUserAuthentication|布尔值|指示配置文件是否需要从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的用户身份验证|
|configurationEndpointUrl|String|用于从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的注册的配置终结点 url|
|enableAuthenticationViaCompanyPortal|布尔值|指示使用 Apple Setup 助理 (而不是公司门户) 进行身份验证。 继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|布尔值|指示在从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的安装助理注册设备上需要公司门户|
|isDefault|Boolean|指示这是否为默认配置文件|
|supervisedModeEnabled|布尔值|监督模式, 如果启用, 则为 True, 否则为 false。 有关https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune详细信息, 请参阅。|
|supportDepartment|String|支持部门信息|
|passCodeDisabled|布尔值|指示是否禁用密码设置窗格|
|isMandatory|布尔值|指示配置文件是否是必需的|
|locationDisabled|布尔值|指示是否禁用位置服务设置窗格|
|supportPhoneNumber|String|支持电话号码|
|iTunesPairingMode|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)|指示 iTunes 配对模式。 可取值为：`disallow`、`allow`、`requiresCertificate`。|
|profileRemovalDisabled|布尔值|指示是否禁用了配置文件删除选项|
|managementCertificates|[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)集合|Apple 配置器的管理证书|
|restoreBlocked|布尔值|指示是否阻止还原安装程序窗格|
|restoreFromAndroidDisabled|布尔值|指示是否禁用从 Android 还原|
|appleIdDisabled|布尔值|指示是否禁用 Apple id 设置窗格|
|termsAndConditionsDisabled|布尔值|指示是否已禁用 "条款和条件" 安装窗格|
|touchIdDisabled|布尔值|指示是否禁用了触控 id 设置窗格|
|applePayDisabled|布尔值|指示是否禁用 Apple 付费设置窗格|
|zoomDisabled|布尔值|指示是否禁用缩放设置窗格|
|siriDisabled|布尔值|指示是否禁用 siri 安装程序窗格|
|diagnosticsDisabled|布尔值|指示是否禁用诊断设置窗格|
|macOSRegistrationDisabled|布尔值|指示是否禁用 Mac OS 注册|
|macOSFileVaultDisabled|布尔值|指示是否禁用 Mac OS 文件保管库|
|awaitDeviceConfiguredConfirmation|布尔值|指示设备是否需要等待已配置的确认|
|sharedIPadMaximumUserCount|Int32|这指定了可以使用共享 iPad 的最大用户数。 仅适用于共享 iPad 模式。|
|enableSharedIPad|布尔值|这表示设备是否要在启用多用户方案的模式中进行注册。 仅适用于共享 ipad。|



## <a name="response"></a>响应
如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
Content-type: application/json
Content-length: 1354

{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "Support Department value",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "iTunesPairingMode": "allow",
  "profileRemovalDisabled": true,
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreBlocked": true,
  "restoreFromAndroidDisabled": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "macOSRegistrationDisabled": true,
  "macOSFileVaultDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1403

{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
  "id": "3d4534f7-34f7-3d45-f734-453df734453d",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "Support Department value",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "iTunesPairingMode": "allow",
  "profileRemovalDisabled": true,
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreBlocked": true,
  "restoreFromAndroidDisabled": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "macOSRegistrationDisabled": true,
  "macOSFileVaultDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true
}
```





